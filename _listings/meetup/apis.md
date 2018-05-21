---
name: Meetup
x-slug: meetup
description: Meetup is an online social networking portal that facilitates offline
  group meetings in various localities around the world. Meetup allows members to
  find and join groups unified by a common interest, such as politics, books, games,
  movies, health, pets, careers or hobbies.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
x-kinRank: "9"
x-alexaRank: ""
tags: Venues
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup Venues
  x-api-slug: meetup
  description: Search for Meetup venues by one of your groups, events, or venue identifiers.
    For a full text search on public venues use [OpenVenues](/meetup_api/docs/2/open_venues).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: http://www.meetup.com/
  baseURL: https://api.meetup.com////2/venues
  tags: Events,Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/meetup/2venues-get-openapi.md
- name: Meetup Find Venues
  x-api-slug: meetup
  description: Returns list of venues based on location
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: http://www.meetup.com/
  baseURL: https://api.meetup.com////find/venues
  tags: Events,Search,Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/meetup/findvenues-get-openapi.md
- name: Meetup Recommended Venues
  x-api-slug: meetup
  description: Returns venues Meetup finds relevant to you based on location and category.
    This method does not yet support sorting or pagination.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: http://www.meetup.com/
  baseURL: https://api.meetup.com////recommended/venues
  tags: Events,Recomendations,Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/meetup/recommendedvenues-get-openapi.md
- name: Meetup
  x-api-slug: meetup
  description: Meetup is an online social networking portal that facilitates offline
    group meetings in various localities around the world. Meetup allows members to
    find and join groups unified by a common interest, such as politics, books, games,
    movies, health, pets, careers or hobbies.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: http://www.meetup.com/
  baseURL: https://api.meetup.com//
  tags: Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/meetup/openapi.md
x-common:
- type: x-base
  url: http://api.meetup.com
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-website
  url: http://www.meetup.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---