---
name: Foursquare
x-slug: foursquare
description: Foursquare helps you find the perfect places to go with friends. Discover
  the best food, nightlife, and entertainment in your area.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
x-kinRank: "9"
x-alexaRank: "2544"
tags: Venues
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/apis.md
specificationVersion: "0.14"
apis:
- name: Foursquare Get Lists Suggestvenues
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggesttip
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggestvenues
  tags: Lists,Suggestvenues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/listslist-idsuggestvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/listslist-idsuggestvenues-get-openapi.md
- name: Foursquare Get Pages Venues
  x-api-slug: foursquare
  description: /pages/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///pages/{PAGE_ID}/venues
  tags: Pages,Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/pagespage-idvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/pagespage-idvenues-get-openapi.md
- name: Foursquare Post Venues Add
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/add
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesadd-post-openapi.md
- name: Foursquare Get Venues Categories
  x-api-slug: foursquare
  description: /venues/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/categories
  tags: Venues,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuescategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuescategories-get-openapi.md
- name: Foursquare Get Venues Explore
  x-api-slug: foursquare
  description: /venues/categories
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/explore
  tags: Venues,Explore
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesexplore-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesexplore-get-openapi.md
- name: Foursquare Get Venues Managed
  x-api-slug: foursquare
  description: /venues/explore
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/managed
  tags: Venues,Managed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesmanaged-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesmanaged-get-openapi.md
- name: Foursquare Get Venues Search
  x-api-slug: foursquare
  description: /venues/managed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/search
  tags: Venues,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuessearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuessearch-get-openapi.md
- name: Foursquare Get Venues Suggestcompletion
  x-api-slug: foursquare
  description: /venues/search
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/suggestcompletion
  tags: Venues,Suggestcompletion
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuessuggestcompletion-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuessuggestcompletion-get-openapi.md
- name: Foursquare Get Venues Timeseries
  x-api-slug: foursquare
  description: /venues/suggestcompletion
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/timeseries
  tags: Venues,Timeseries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuestimeseries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuestimeseries-get-openapi.md
- name: Foursquare Get Venues Trending
  x-api-slug: foursquare
  description: /venues/timeseries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/trending
  tags: Venues,Trending
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuestrending-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuestrending-get-openapi.md
- name: Foursquare Get Venues
  x-api-slug: foursquare
  description: /users/self/update
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-id-get-openapi.md
- name: Foursquare Post Venues Edit
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/tips
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/edit
  tags: Venues,Edit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idedit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idedit-post-openapi.md
- name: Foursquare Get Venues Events
  x-api-slug: foursquare
  description: /venues/trending
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/events
  tags: Venues,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idevents-get-openapi.md
- name: Foursquare Post Venues Flag
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/edit
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/flag
  tags: Venues,Flag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idflag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idflag-post-openapi.md
- name: Foursquare Get Venues Herenow
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/herenow
  tags: Venues,Herenow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idherenow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idherenow-get-openapi.md
- name: Foursquare Get Venues Links
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/herenow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/links
  tags: Venues,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idlinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idlinks-get-openapi.md
- name: Foursquare Get Venues Listed
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/links
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/listed
  tags: Venues,Listed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idlisted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idlisted-get-openapi.md
- name: Foursquare Post Venues Marktodo
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/flag
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/marktodo
  tags: Venues,Marktodo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idmarktodo-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idmarktodo-post-openapi.md
- name: Foursquare Get Venues Menu
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/listed
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/menu
  tags: Venues,Menu
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idmenu-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idmenu-get-openapi.md
- name: Foursquare Get Venues Photos
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/menu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/photos
  tags: Venues,Photos
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idphotos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idphotos-get-openapi.md
- name: Foursquare Post Venues Proposeedit
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/marktodo
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/proposeedit
  tags: Venues,Proposeedit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idproposeedit-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idproposeedit-post-openapi.md
- name: Foursquare Get Venues Similar
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/photos
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/similar
  tags: Venues,Similar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idsimilar-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idsimilar-get-openapi.md
- name: Foursquare Get Venues Stats
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/similar
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/stats
  tags: Venues,Stats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idstats-get-openapi.md
- name: Foursquare Get Venues Tips
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/stats
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venues/{VENUE_ID}/tips
  tags: Venues,Tips
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idtips-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/venuesvenue-idtips-get-openapi.md
- name: Foursquare
  x-api-slug: foursquare
  description: foursquare makes the real world easier to use. We build tools that
    help you keep up with friends, discover whats nearby, save money and unlock deals.
    Whether youre setting off on a trip around the world, coordinating a night out
    with friends, or trying to pick out the best dish at your local restaurant, foursquare
    is the perfect companion. The foursquare API gives you access to all of the data
    used by the foursquare mobile applications, and, in some cases, even more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2/
  tags: Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/foursquare/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/foursquare.json
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/foursquare/apidescription?format=internal&ver=1393644831000
- type: x-application-management
  url: https://foursquare.com/developers/apps
- type: x-blog
  url: http://engineering.foursquare.com/
- type: x-blog-rss
  url: http://engineering.foursquare.com/feed/
- type: x-curated-source
  url: http://blog.foursquare.com/2013/09/17/we-put-a-fresh-coat-of-paint-on-foursquare-for-ios-7/
- type: x-website
  url: http://blog.foursquare.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/foursquare
- type: x-crunchbase
  url: https://crunchbase.com/organization/foursquare
- type: x-email
  url: support@foursquare.com
- type: x-email
  url: ads@foursquare.com
- type: x-email
  url: press@foursquare.com
- type: x-email
  url: security@foursquare.com
- type: x-email
  url: feedback@foursquare.com
- type: x-email
  url: privacy@foursquare.com
- type: x-error-codes
  url: https://developer.foursquare.com/overview/responses
- type: x-foursquare
  url: http://foursquare.com/nasa
- type: x-foursquare
  url: http://foursquare.com/yourcommissary
- type: x-getting-started
  url: https://developer.foursquare.com/start
- type: x-github
  url: https://github.com/foursquare
- type: x-privacy
  url: https://foursquare.com/legal/privacy
- type: x-rate-limits
  url: https://developer.foursquare.com/overview/ratelimits
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/foursquare
- type: x-terms-of-service
  url: https://developer.foursquare.com/overview/community
- type: x-twitter
  url: https://twitter.com/foursquare
- type: x-twitter
  url: https://twitter.com/foursquareapi
- type: x-website
  url: http://foursquare.com
- type: x-website
  url: https://developer.foursquare.com/
- type: x-website
  url: https://foursquare.com/apps/slack
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---