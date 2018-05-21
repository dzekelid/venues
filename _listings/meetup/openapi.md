---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
  description: the-meetup-api-provides-simple-restful-http-and-streaming-interfaces-for-exploring-and-interacting-meetup-platform-from-your-own-apps-the-api-is-a-set-of-core-methods-and-a-common-request-format-these-are-combined-to-form-a-url-that-returns-the-information-you-want-
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
---