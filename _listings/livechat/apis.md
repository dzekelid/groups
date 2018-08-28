---
name: LiveChat
x-slug: livechat
description: LiveChat is an offline customer service software with live support, help
  desk software, and web analytics capabilities.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
x-kinRank: "7"
x-alexaRank: "4371"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/apis.md
specificationVersion: "0.14"
apis:
- name: LiveChat REST API - List all groups
  x-api-slug: groups-get
  description: Returns all created groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
  humanURL: https://www.livechatinc.com/
  baseURL: https://api.livechatinc.com//
  tags: SaaS, Technology, Support, Chats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groups-get-openapi.md
- name: LiveChat REST API - Get a single group details
  x-api-slug: groupsgroup-id-get
  description: Returns group details for the given GROUP_ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
  humanURL: https://www.livechatinc.com/
  baseURL: https://api.livechatinc.com//
  tags: SaaS, Technology, Support, Chats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsgroup-id-get-openapi.md
- name: LiveChat REST API - Create a new group
  x-api-slug: groups-post
  description: Creates a new group in your license.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
  humanURL: https://www.livechatinc.com/
  baseURL: https://api.livechatinc.com//
  tags: SaaS, Technology, Support, Chats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groups-post-openapi.md
- name: LiveChat REST API - Remove a group
  x-api-slug: groupsabc123-delete
  description: Removes a group with the given GROUP_ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
  humanURL: https://www.livechatinc.com/
  baseURL: https://api.livechatinc.com//
  tags: SaaS, Technology, Support, Chats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsabc123-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsabc123-delete-openapi.md
- name: LiveChat REST API - Update a group
  x-api-slug: groupsabc123-put
  description: Updates the specified group by setting the values of the parameters
    passed. Any parameters not provided will be left unchanged.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28877-developers-livechatinc-com.jpg
  humanURL: https://www.livechatinc.com/
  baseURL: https://api.livechatinc.com//
  tags: SaaS, Technology, Support, Chats
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsabc123-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/livechat/groupsabc123-put-openapi.md
x-common:
- type: x-website
  url: https://www.livechatinc.com/
- type: x-api-gallery
  url: http://lisk.api.gallery.streamdata.io
- type: x-crunchbase
  url: https://crunchbase.com/organization/livechatsoftware
- type: x-email
  url: support@livechatinc.com
- type: x-twitter
  url: https://twitter.com/LiveChat
- type: x-developer
  url: https://developers.livechatinc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---