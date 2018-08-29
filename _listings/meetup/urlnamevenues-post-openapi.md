---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Venue Create
  description: Interface for creating new Meetup venues
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/venues:
    get:
      summary: Venues
      description: Search for Meetup venues by one of your groups, events, or venue
        identifiers. For a full text search on public venues use [OpenVenues](/meetup_api/docs/2/open_venues).
      operationId: venues
      x-api-path-slug: 2venues-get
      parameters:
      - in: query
        name: event_id
        description: multiple ids may be separated with commas
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_id
        description: multiple ids may be separated with commas
        type: string
      - in: query
        name: group_urlname
        description: path to group from meetup
        type: string
      - in: query
        name: venue_id
        description: multiple ids may be separated with commas
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Venues
  /find/venues:
    get:
      summary: Find Venues
      description: Returns list of venues based on location
      operationId: venues
      x-api-path-slug: findvenues-get
      parameters:
      - in: query
        name: country
        description: A valid two charater country code, desfaults to US
        type: string
      - in: query
        name: desc
        description: Boolean value to indicate to direction ordered results
        type: string
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: lat
        description: Approximate latitude
        type: string
      - in: query
        name: location
        description: Raw text location query
        type: string
      - in: query
        name: lon
        description: Approximate longitude
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: text
        description: Raw full text search query
        type: string
      - in: query
        name: zip
        description: Zipcode of location to limit search to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Venues
  /recommended/venues:
    get:
      summary: Recommended Venues
      description: Returns venues Meetup finds relevant to you based on location and
        category. This method does not yet support sorting or pagination.
      operationId: venues
      x-api-path-slug: recommendedvenues-get
      parameters:
      - in: query
        name: category
        description: Comma-delimited list of up to 200 category ids to help inform
          recommendations
        type: string
      - in: query
        name: country
        description: A valid two character country code, defaults to US
        type: string
      - in: query
        name: group_id
        description: Comma-delimited list of up to 200 group ids to help inform recommendations
        type: string
      - in: query
        name: group_urlname
        description: Comma-delimited list of up to 200 group urlnames to help inform
          recommendations
        type: string
      - in: query
        name: lat
        description: Approximate latitude
        type: string
      - in: query
        name: location
        description: Raw text location query
        type: string
      - in: query
        name: lon
        description: Approximate longitude
        type: string
      - in: query
        name: min_groups
        description: The minimum number of groups that have hosted events at this
          venue
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: used_between
        description: Return venues that have been used within the given time range,
          defined by two times separated with a single comma
        type: string
      - in: query
        name: zip
        description: Zip code you are searching for recommendations in
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Recomendations
      - Venues
  /2/open_venues:
    get:
      summary: OpenVenues
      description: Searches for public venues within a given geo space. To search
        for specific venues that your group has used, use the [Venues](/meetup_api/docs/2/venues)
        method
      operationId: venues
      x-api-path-slug: 2open-venues-get
      parameters:
      - in: query
        name: api_version
        description: "2"
        type: string
      - in: query
        name: city
        description: A valid city
        type: string
      - in: query
        name: country
        description: A valid country code
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_urlname
        description: Returns venues with location relative to the group associated
          with this urlname
        type: string
      - in: query
        name: lat
        description: A valid latitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: lon
        description: A valid longitude, limits the returned venues to those within
          radius miles
        type: string
      - in: query
        name: radius
        description: Radius, in miles for geographic requests, default 25
        type: string
      - in: query
        name: since_count
        description: Request that some number of recent messages be sent immediately,
          if available
        type: string
      - in: query
        name: since_mtime
        description: Return recent open venues with an mtime greater then the supplied
          time, in milliseconds since the epoch
        type: string
      - in: query
        name: state
        description: For the US, a valid 2 character state code
        type: string
      - in: query
        name: text
        description: Venues that contain the given term or terms somewhere in their
          content
        type: string
      - in: query
        name: trickle
        description: When supplied with a request, the Meetup API will push your client
          the entire Meetup database of public venues in batches of 512
        type: string
      - in: query
        name: zip
        description: A valid US zip code, limits the returned venues to those within
          radius miles
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
  /:urlname/venues:
    get:
      summary: Group Venues
      description: Returns venues a group has previously hosted events at
      operationId: venues
      x-api-path-slug: urlnamevenues-get
      parameters:
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Veues
    post:
      summary: Venue Create
      description: Interface for creating new Meetup venues
      operationId: venues
      x-api-path-slug: urlnamevenues-post
      parameters:
      - in: query
        name: address_1
        description: Primary address of the venue
        type: string
      - in: query
        name: address_2
        description: Secondary address info
        type: string
      - in: query
        name: city
        description: City name of the venue
        type: string
      - in: query
        name: country
        description: 2 character country code of the venue
        type: string
      - in: query
        name: fields
        description: Comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: hours
        description: Open hours information about the venue
        type: string
      - in: query
        name: name
        description: Unique name of the venue
        type: string
      - in: query
        name: phone
        description: Optional phone number for the venue
        type: string
      - in: query
        name: state
        description: If in the US or CA, the state code for the venue
        type: string
      - in: query
        name: visibility
        description: Optional value indicating the venues visibility to others
        type: string
      - in: query
        name: web_url
        description: Optional web url for the venue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Photos
      - Veues
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