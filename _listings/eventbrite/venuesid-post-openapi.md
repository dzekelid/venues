---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Add Venues
  description: Updates a venue and returns it as an object.
  version: 1.0.0
host: www.eventbriteapi.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/venues/:
    get:
      summary: Get Users  Venues
      description: Returns a paginated response of venue objects that are owned by
        the user.
      operationId: getUsersVenues
      x-api-path-slug: usersidvenues-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Venues
  /organizations/{id}/venues/:
    post:
      summary: Add Organizations  Venues
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
      - ""
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
      summary: Add Venues
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---