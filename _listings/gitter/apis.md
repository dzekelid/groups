---
name: Gitter
x-slug: gitter
description: Gitter is a chat and networking platform that helps to manage, grow and
  connect communities through messaging, content and discovery.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
x-kinRank: "8"
x-alexaRank: "18282"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/apis.md
specificationVersion: "0.14"
apis:
- name: Gitter API List Groups
  x-api-slug: gitter-api
  description: List groups the current user is in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///groups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/groups-get-openapi.md
- name: Gitter API Group Rooms
  x-api-slug: gitter-api
  description: List rooms under group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///groups/:groupId/rooms
  tags: Groups,Rooms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/groupsgroupidrooms-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/groupsgroupidrooms-get-openapi.md
- name: Gitter API
  x-api-slug: gitter-api
  description: Gitter is a chat and networking platform that helps to manage, grow
    and connect communities through messaging, content and discovery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https:///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gitter/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/gitter
- type: x-developer
  url: https://developer.gitter.im/docs/streaming-api
- type: x-github
  url: https://github.com/gitterHQ
- type: x-curated-source
  url: https://gitter.im/apiaryio/api-blueprint
- type: x-website
  url: http://gitter.im
- type: x-twitter
  url: https://twitter.com/gitchat
- type: x-website
  url: https://gitter.im
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---