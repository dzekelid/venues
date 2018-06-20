---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Venues Links
  description: /venues/{VENUE_ID}/herenow
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{LIST_ID}/suggestvenues:
    get:
      summary: Get Lists Suggestvenues
      description: /lists/{LIST_ID}/suggesttip
      operationId: listslist-idsuggesttip
      x-api-path-slug: listslist-idsuggestvenues-get
      parameters:
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestvenues
  /pages/{PAGE_ID}/venues:
    get:
      summary: Get Pages Venues
      description: /pages/search
      operationId: pagessearch
      x-api-path-slug: pagespage-idvenues-get
      parameters:
      - in: query
        name: limit
        description: The number of venues to return
      - in: query
        name: ll
        description: Not valid with ne or sw
      - in: query
        name: ne
        description: See sw
      - in: query
        name: offset
        description: The offset of which venues to return
      - in: query
        name: PAGE_ID
        description: The page id for which venues are being requested
      - in: path
        name: PAGE_ID
      - in: query
        name: radius
        description: Can be used when including ll
      - in: query
        name: sw
        description: With ne, limits results to the bounding quadrangle defined by
          the latitude and longitude given by sw as its south-west corner, and ne
          as its north-east corner
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Venues
  /venues/add:
    post:
      summary: Post Venues Add
      description: /venues/{VENUE_ID}
      operationId: venuesvenue-id
      x-api-path-slug: venuesadd-post
      parameters:
      - in: query
        name: address
        description: The address of the venue
      - in: query
        name: city
        description: The city name where this venue is
      - in: query
        name: crossStreet
        description: The nearest intersecting street or streets
      - in: query
        name: description
        description: A freeform description of the venue, up to 300 characters
      - in: query
        name: ignoreDuplicates
        description: A boolean flag telling the server to ignore duplicates and force
          the addition of this venue
      - in: query
        name: ignoreDuplicatesKey
        description: Required if ignoreDuplicates is true
      - in: query
        name: ll
        description: Latitude and longitude of the venue, as accurate as is known
      - in: query
        name: name
        description: The name of the venue
      - in: query
        name: phone
        description: The phone number of the venue
      - in: query
        name: primaryCategoryId
        description: The ID of the category to which you want to assign this venue
      - in: query
        name: state
        description: The nearest state or province to the venue
      - in: query
        name: twitter
        description: The twitter handle of the venue
      - in: query
        name: url
        description: The url of the homepage of the venue
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: zip
        description: The zip or postal code for the venue
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/categories:
    get:
      summary: Get Venues Categories
      description: /venues/add
      operationId: venuesadd
      x-api-path-slug: venuescategories-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Categories
  /venues/explore:
    get:
      summary: Get Venues Explore
      description: /venues/categories
      operationId: venuescategories
      x-api-path-slug: venuesexplore-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: intent
        description: Limit results to venues with specials
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude of the users location, so response can
          include distance
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: novelty
        description: Pass new or old to limit results to places the acting user hasnt
          been or has been, respectively
      - in: query
        name: query
        description: A search term to be applied against tips, category, tips, etc
      - in: query
        name: radius
        description: Radius to search within, in meters
      - in: query
        name: section
        description: One of food, drinks, coffee, shops, arts, or outdoors
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Explore
  /venues/managed:
    get:
      summary: Get Venues Managed
      description: /venues/explore
      operationId: venuesexplore
      x-api-path-slug: venuesmanaged-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Managed
  /venues/search:
    get:
      summary: Get Venues Search
      description: /venues/managed
      operationId: venuesmanaged
      x-api-path-slug: venuessearch-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: categoryId
        description: A comma separated list of categories to limit results to
      - in: query
        name: intent
        description: One of the values checkin, browse or match, indicating your intent
          in performing the search
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: linkedId
        description: Identifier used by third party specified in providerId, which
          we will attempt to match against our map of venues to URLs
      - in: query
        name: ll
        description: Latitude and longitude of the users location, so response can
          include distance
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: ne
        description: See sw
      - in: query
        name: providerId
        description: Identifier for a known third party that is part of our map of
          venues to URLs, used in conjunction with linkedId
      - in: query
        name: query
        description: A search term to be applied against venue names
      - in: query
        name: radius
        description: Limit results to venues within this many meters of the specified
          location
      - in: query
        name: sw
        description: With ne, limits results to the bounding quadrangle defined by
          the latitude and longitude given by sw as its south-west corner, and ne
          as its north-east corner
      - in: query
        name: url
        description: A third-party URL which we will attempt to match against our
          map of venues to URLs
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Search
  /venues/suggestcompletion:
    get:
      summary: Get Venues Suggestcompletion
      description: /venues/search
      operationId: venuessearch
      x-api-path-slug: venuessuggestcompletion-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: limit
        description: Number of results to return, up to 100
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: query
        description: A search term to be applied against titles
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Suggestcompletion
  /venues/timeseries:
    get:
      summary: Get Venues Timeseries
      description: /venues/suggestcompletion
      operationId: venuessuggestcompletion
      x-api-path-slug: venuestimeseries-get
      parameters:
      - in: query
        name: endAt
        description: The end of the time range to retrieve stats for (seconds since
          epoch)
      - in: query
        name: startAt
        description: The start of the time range to retrieve stats for (seconds since
          epoch)
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: A comma-separated list of venue ids to retrieve series data for
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Timeseries
  /venues/trending:
    get:
      summary: Get Venues Trending
      description: /venues/timeseries
      operationId: venuestimeseries
      x-api-path-slug: venuestrending-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude of the users location
      - in: query
        name: radius
        description: Radius in meters, up to approximately 2000 meters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Trending
  /venues/{VENUE_ID}:
    get:
      summary: Get Venues
      description: /users/self/update
      operationId: usersselfupdate
      x-api-path-slug: venuesvenue-id-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: ID of venue to retrieve
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
  /venues/{VENUE_ID}/edit:
    post:
      summary: Post Venues Edit
      description: /venues/{VENUE_ID}/tips
      operationId: venuesvenue-idtips
      x-api-path-slug: venuesvenue-idedit-post
      parameters:
      - in: query
        name: address
        description: The address of the venue
      - in: query
        name: categoryId
        description: The IDs of the category or categories to which you want to assign
          this venue (separate multiple IDs with commas)
      - in: query
        name: city
        description: The city name where this venue is
      - in: query
        name: crossStreet
        description: The nearest intersecting street or streets
      - in: query
        name: description
        description: A freeform description of the venue, up to 300 characters
      - in: query
        name: ll
        description: Latitude and longitude of the venue
      - in: query
        name: name
        description: The name of the venue
      - in: query
        name: phone
        description: The phone number of the venue
      - in: query
        name: state
        description: The nearest state or province to the venue
      - in: query
        name: twitter
        description: The twitter handle of the venue
      - in: query
        name: url
        description: The url of the homepage of the venue
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: The venue id to edit
      - in: path
        name: VENUE_ID
      - in: query
        name: zip
        description: The zip or postal code for the venue
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Edit
  /venues/{VENUE_ID}/events:
    get:
      summary: Get Venues Events
      description: /venues/trending
      operationId: venuestrending
      x-api-path-slug: venuesvenue-idevents-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: The venue id for which events are being requested
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Events
  /venues/{VENUE_ID}/flag:
    post:
      summary: Post Venues Flag
      description: /venues/{VENUE_ID}/edit
      operationId: venuesvenue-idedit
      x-api-path-slug: venuesvenue-idflag-post
      parameters:
      - in: query
        name: problem
        description: One of mislocated, closed, duplicate, inappropriate, doesnt_exist,
          event_over
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: ID of the duplicated venue (for problem duplicate)
      - in: query
        name: VENUE_ID
        description: The venue id for which an edit is being proposed
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Flag
  /venues/{VENUE_ID}/herenow:
    get:
      summary: Get Venues Herenow
      description: /venues/{VENUE_ID}/events
      operationId: venuesvenue-idevents
      x-api-path-slug: venuesvenue-idherenow-get
      parameters:
      - in: query
        name: afterTimestamp
        description: Retrieve the first results to follow these seconds since epoch
      - in: query
        name: limit
        description: Number of results to return, up to 500
      - in: query
        name: offset
        description: Used to page through results
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: ID of venue to retrieve
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Herenow
  /venues/{VENUE_ID}/links:
    get:
      summary: Get Venues Links
      description: /venues/{VENUE_ID}/herenow
      operationId: venuesvenue-idherenow
      x-api-path-slug: venuesvenue-idlinks-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: VENUE_ID
        description: The venue you want annotations for
      - in: path
        name: VENUE_ID
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Links
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