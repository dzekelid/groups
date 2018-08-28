---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Groups Members. Format
  description: Returns a collection of members of the group with group id
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/groups.json:
    get:
      summary: Get Users Groups
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.json
      x-api-path-slug: usersuser-idgroups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /me/groups.json:
    get:
      summary: Get Me Groups
      description: Returns a collection of groups joined by logged-in user
      operationId: getMeGroups.json
      x-api-path-slug: megroups-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Groups
  /groups.json:
    get:
      summary: Get Groups
      description: Returns a collection of groups
      operationId: getGroups.json
      x-api-path-slug: groups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}.json:
    get:
      summary: Get Groups
      description: Returns a group by group id
      operationId: getGroupsGroup.json
      x-api-path-slug: groupsgroup-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}/users.json:
    get:
      summary: Get Groups Users
      description: Returns a combined collection of moderators, members and contributors
        of the group with group id
      operationId: getGroupsGroupUsers.json
      x-api-path-slug: groupsgroup-idusers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Users
  /groups/{group_id}/moderators.json:
    get:
      summary: Get Groups Moderators
      description: Returns a collection of moderators of the group with group id
      operationId: getGroupsGroupModerators.json
      x-api-path-slug: groupsgroup-idmoderators-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Moderators
  /groups/{group_id}/members.json:
    get:
      summary: Get Groups Members
      description: Returns a collection of members of the group with group id
      operationId: getGroupsGroupMembers.json
      x-api-path-slug: groupsgroup-idmembers-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
  /groups/{group_id}/contributors.json:
    get:
      summary: Get Groups Contributors
      description: Returns a collection of contributors of the group with group id
      operationId: getGroupsGroupContributors.json
      x-api-path-slug: groupsgroup-idcontributors-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Contributors
  /groups/{group_id}/tracks.json:
    get:
      summary: Get Groups Tracks
      description: Returns a collection of tracks contributed to the group with group
        id
      operationId: getGroupsGroupTracks.json
      x-api-path-slug: groupsgroup-idtracks-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Tracks
  /users/{user_id}/groups.{format}:
    get:
      summary: Get Users Groups. Format
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.Format
      x-api-path-slug: usersuser-idgroups-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
      - ""
      - Format
  /me/groups.{format}:
    get:
      summary: Get Me Groups. Format
      description: Returns a collection of groups joined by logged-in user
      operationId: getMeGroups.Format
      x-api-path-slug: megroups-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Groups
      - ""
      - Format
  /groups.{format}:
    get:
      summary: Get Groups. Format
      description: Returns a collection of groups
      operationId: getGroups.Format
      x-api-path-slug: groups-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - ""
      - Format
  /groups/{group_id}.{format}:
    get:
      summary: Get Groups . Format
      description: Returns a group by group id
      operationId: getGroupsGroup.Format
      x-api-path-slug: groupsgroup-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - ""
      - ""
      - Format
  /groups/{group_id}/users.{format}:
    get:
      summary: Get Groups Users. Format
      description: Returns a combined collection of moderators, members and contributors
        of the group with group id
      operationId: getGroupsGroupUsers.Format
      x-api-path-slug: groupsgroup-idusers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Users
      - ""
      - Format
  /groups/{group_id}/moderators.{format}:
    get:
      summary: Get Groups Moderators. Format
      description: Returns a collection of moderators of the group with group id
      operationId: getGroupsGroupModerators.Format
      x-api-path-slug: groupsgroup-idmoderators-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Moderators
      - ""
      - Format
  /groups/{group_id}/members.{format}:
    get:
      summary: Get Groups Members. Format
      description: Returns a collection of members of the group with group id
      operationId: getGroupsGroupMembers.Format
      x-api-path-slug: groupsgroup-idmembers-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - ""
      - Format
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