---
name: SoundCloud
x-slug: soundcloud
description: SoundCloud is a music and podcast streaming platform that lets you listen
  to millions of songs from around the world, or upload your own. Start listening
  now!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
x-kinRank: "9"
x-alexaRank: "112"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/apis.md
specificationVersion: "0.14"
apis:
- name: Sound Cloud Get Users Groups
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/groups.json
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/usersuser-idgroups-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/usersuser-idgroups-json-get-openapi.md
- name: Sound Cloud Get Me Groups
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by logged-in user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////me/groups.json
  tags: Me,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/megroups-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/megroups-json-get-openapi.md
- name: Sound Cloud Get Groups
  x-api-slug: sound-cloud
  description: Returns a collection of groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups.json
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groups-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groups-json-get-openapi.md
- name: Sound Cloud Get Groups
  x-api-slug: sound-cloud
  description: Returns a group by group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}.json
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-id-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-id-json-get-openapi.md
- name: Sound Cloud Get Groups Users
  x-api-slug: sound-cloud
  description: Returns a combined collection of moderators, members and contributors
    of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/users.json
  tags: Groups,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idusers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idusers-json-get-openapi.md
- name: Sound Cloud Get Groups Moderators
  x-api-slug: sound-cloud
  description: Returns a collection of moderators of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/moderators.json
  tags: Groups,Moderators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmoderators-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmoderators-json-get-openapi.md
- name: Sound Cloud Get Groups Members
  x-api-slug: sound-cloud
  description: Returns a collection of members of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/members.json
  tags: Groups,Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmembers-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmembers-json-get-openapi.md
- name: Sound Cloud Get Groups Contributors
  x-api-slug: sound-cloud
  description: Returns a collection of contributors of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/contributors.json
  tags: Groups,Contributors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idcontributors-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idcontributors-json-get-openapi.md
- name: Sound Cloud Get Groups Tracks
  x-api-slug: sound-cloud
  description: Returns a collection of tracks contributed to the group with group
    id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/tracks.json
  tags: Groups,Tracks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idtracks-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idtracks-json-get-openapi.md
- name: Sound Cloud Get Users Groups. Format
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by user with user id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////users/{user_id}/groups.{format}
  tags: Users,Groups,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/usersuser-idgroups-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/usersuser-idgroups-format-get-openapi.md
- name: Sound Cloud Get Me Groups. Format
  x-api-slug: sound-cloud
  description: Returns a collection of groups joined by logged-in user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////me/groups.{format}
  tags: Me,Groups,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/megroups-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/megroups-format-get-openapi.md
- name: Sound Cloud Get Groups. Format
  x-api-slug: sound-cloud
  description: Returns a collection of groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups.{format}
  tags: Groups,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groups-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groups-format-get-openapi.md
- name: Sound Cloud Get Groups . Format
  x-api-slug: sound-cloud
  description: Returns a group by group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}.{format}
  tags: Groups,,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-id-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-id-format-get-openapi.md
- name: Sound Cloud Get Groups Users. Format
  x-api-slug: sound-cloud
  description: Returns a combined collection of moderators, members and contributors
    of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/users.{format}
  tags: Groups,Users,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idusers-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idusers-format-get-openapi.md
- name: Sound Cloud Get Groups Moderators. Format
  x-api-slug: sound-cloud
  description: Returns a collection of moderators of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/moderators.{format}
  tags: Groups,Moderators,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmoderators-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmoderators-format-get-openapi.md
- name: Sound Cloud Get Groups Members. Format
  x-api-slug: sound-cloud
  description: Returns a collection of members of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/members.{format}
  tags: Groups,Members,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmembers-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idmembers-format-get-openapi.md
- name: Sound Cloud Get Groups Contributors. Format
  x-api-slug: sound-cloud
  description: Returns a collection of contributors of the group with group id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/contributors.{format}
  tags: Groups,Contributors,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idcontributors-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idcontributors-format-get-openapi.md
- name: Sound Cloud Get Groups Tracks. Format
  x-api-slug: sound-cloud
  description: Returns a collection of tracks contributed to the group with group
    id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com////groups/{group_id}/tracks.{format}
  tags: Groups,Tracks,,Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idtracks-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/groupsgroup-idtracks-format-get-openapi.md
- name: Sound Cloud
  x-api-slug: sound-cloud
  description: SoundCloud is a music and podcast streaming platform that lets you
    listen to millions of songs from around the world, or upload your own. Start listening
    now!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/252-soundcloud.jpg
  humanURL: http://soundcloud.com
  baseURL: https://api.soundcloud.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/soundcloud/openapi.md
x-common:
- type: x-base
  url: https://api.soundcloud.com
- type: x-blog
  url: http://blog.soundcloud.com
- type: x-blog-rss
  url: http://blog.soundcloud.com/feed/
- type: x-console
  url: https://developers.soundcloud.com/console
- type: x-crunchbase
  url: https://crunchbase.com/organization/soundcloud
- type: x-crunchbase
  url: http://www.crunchbase.com/company/soundcloud
- type: x-developer
  url: http://developers.soundcloud.com
- type: x-github
  url: https://github.com/soundcloud
- type: x-linkedin
  url: https://www.linkedin.com/company/soundcloud/
- type: x-pricing
  url: https://on.soundcloud.com/
- type: x-privacy
  url: https://soundcloud.com/pages/privacy
- type: x-support
  url: https://soundcloud.com/imprint
- type: x-terms-of-service
  url: https://soundcloud.com/terms-of-use
- type: x-twitter
  url: https://twitter.com/soundcloudapi
- type: x-twitter
  url: https://twitter.com/SoundCloud
- type: x-website
  url: http://soundcloud.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---