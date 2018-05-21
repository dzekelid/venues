---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite believes that anyone can be an event organizer. That&rsquo;s
  why they offer tools that make it easy to sell tickets to all kinds of events whether
  it&rsquo;s a photography class or a sold-out concert, an inspiring conference or
  an air-guitar competition. With Eventbrite, organizers can create a customizable
  event page; spread the word with social media; collect money; and gain visibility
  into attendees and sales. Eventbrite is for anyone planning or attending an event.
  It empowers event organizers to become more efficient and effective when bringing
  people together. And people everywhere are searching Eventbrite to discover great
  events that matter to them.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
x-kinRank: "9"
x-alexaRank: ""
tags: Venues
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Get Users  Venues
  x-api-slug: eventbrite
  description: Returns a paginated response of venue objects that are owned by the
    user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//users/{id}/venues/
  tags: Users,,Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/usersidvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/usersidvenues-get-openapi.md
- name: Eventbrite Add Organizations  Venues
  x-api-slug: eventbrite
  description: Creates new venue objects under an organization and returns it as venue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//organizations/{id}/venues/
  tags: Organizations,,Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/organizationsidvenues-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/organizationsidvenues-post-openapi.md
- name: Eventbrite Get Venues
  x-api-slug: eventbrite
  description: Returns a venue object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//venues/{id}/
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesid-get-openapi.md
- name: Eventbrite Add Venues
  x-api-slug: eventbrite
  description: Updates a venue and returns it as an object.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//venues/{id}/
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesid-post-openapi.md
- name: Eventbrite Add Venues
  x-api-slug: eventbrite
  description: Creates a new venue with associated address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//venues/
  tags: Venues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venues-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venues-post-openapi.md
- name: Eventbrite Get Venues  Events
  x-api-slug: eventbrite
  description: Returns events of a given venue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3//venues/{id}/events/
  tags: Venues,,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/venuesidevents-get-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite believes that anyone can be an event organizer. That&rsquo;s
    why they offer tools that make it easy to sell tickets to all kinds of events
    whether it&rsquo;s a photography class or a sold-out concert, an inspiring conference
    or an air-guitar competition. With Eventbrite, organizers can create a customizable
    event page; spread the word with social media; collect money; and gain visibility
    into attendees and sales. Eventbrite is for anyone planning or attending an event.
    It empowers event organizers to become more efficient and effective when bringing
    people together. And people everywhere are searching Eventbrite to discover great
    events that matter to them.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/eventbritelogoff8000gradient.png
  humanURL: http://developer.eventbrite.com/
  baseURL: https://www.eventbriteapi.com//v3
  tags: Venues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/venues/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdksio
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-website
  url: http://developer.eventbrite.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---