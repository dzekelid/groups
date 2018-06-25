---
name: Foursquare
x-slug: foursquare
description: Foursquare helps you find the perfect places to go with friends. Discover
  the best food, nightlife, and entertainment in your area.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
x-kinRank: "9"
x-alexaRank: "2544"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/apis.md
specificationVersion: "0.14"
apis:
- name: Foursquare Post Venuegroups Add
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/add
  tags: Venuegroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsadd-post-openapi.md
- name: Foursquare Get Venuegroups List
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}/delete
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/list
  tags: Venuegroups,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupslist-get-openapi.md
- name: Foursquare Get Venuegroups Group
  x-api-slug: foursquare
  description: /venues/{VENUE_ID}/proposeedit
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}
  tags: Venuegroups,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-id-get-openapi.md
- name: Foursquare Post Venuegroups Group Addvenue
  x-api-slug: foursquare
  description: /venuegroups/list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/addvenue
  tags: Venuegroups,Group,Venue
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-idaddvenue-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-idaddvenue-post-openapi.md
- name: Foursquare Post Venuegroups Group Delete
  x-api-slug: foursquare
  description: /venuegroups/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/delete
  tags: Venuegroups,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-iddelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-iddelete-post-openapi.md
- name: Foursquare Post Venuegroups Group Removevenue
  x-api-slug: foursquare
  description: /venuegroups/{GROUP_ID}/addvenue
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///venuegroups/{GROUP_ID}/removevenue
  tags: Venuegroups,Group,Removevenue
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-idremovevenue-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/venuegroupsgroup-idremovevenue-post-openapi.md
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
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/foursquare/openapi.md
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