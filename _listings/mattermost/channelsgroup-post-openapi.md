---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Create a group message channel
  description: |-
    Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
    ##### Permissions
    Must have `create_group_channel` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels/group:
    post:
      summary: Create a group message channel
      description: |-
        Create a new group message channel to group of users. If the logged in user's id is not included in the list, it will be appended to the end.
        ##### Permissions
        Must have `create_group_channel` permission.
      operationId: create-a-new-group-message-channel-to-group-of-users-if-the-logged-in-users-id-is-not-included-in-th
      x-api-path-slug: channelsgroup-post
      parameters:
      - in: body
        name: body
        description: User ids to be in the group message channel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Group
      - Message
      - Channel
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