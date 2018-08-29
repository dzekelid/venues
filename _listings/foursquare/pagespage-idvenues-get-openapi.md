---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Pages Venues
  description: /pages/search
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