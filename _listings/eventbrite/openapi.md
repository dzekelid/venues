---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/venues/:
    get:
      summary: Get Users Venues
      description: Returns a paginated response of venue objects that are owned by
        the user.
      operationId: getUsersVenues
      x-api-path-slug: usersidvenues-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Venues
  /organizations/{id}/venues/:
    post:
      summary: Post Organizations Venues
      description: Creates new venue objects under an organization and returns it
        as venue.
      operationId: postOrganizationsVenues
      x-api-path-slug: organizationsidvenues-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Venues
  /venues/{id}/:
    get:
      summary: Get Venues
      description: Returns a venue object.
      operationId: getVenues
      x-api-path-slug: venuesid-get
      responses:
        200:
          description: OK
      tags:
      - Venues
    post:
      summary: Post Venues
      description: Updates a venue and returns it as an object.
      operationId: postVenues
      x-api-path-slug: venuesid-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/:
    post:
      summary: Post Venues
      description: Creates a new venue with associated address.
      operationId: postVenues
      x-api-path-slug: venues-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/{id}/events/:
    get:
      summary: Get Venues Events
      description: Returns events of a given venue.
      operationId: getVenuesEvents
      x-api-path-slug: venuesidevents-get
      parameters:
      - in: query
        name: only_public
        description: Only show public events even if viewing your own events
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: start_date.range_end
        description: Only return events with start dates before the given date
        type: query
      - in: query
        name: start_date.range_start
        description: Only return events with start dates after the given date
        type: query
      - in: query
        name: status
        description: Only return events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Events
  /user_list_venues:
    get:
      summary: Get User List Venues
      description: This method lists the venues created by this user. Requires authentication.
      operationId: Get_user_list_venues_
      x-api-path-slug: user-list-venues-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Venues
---