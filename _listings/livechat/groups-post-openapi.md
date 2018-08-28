---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Create a new group
  description: Creates a new group in your license.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: List all groups
      description: Returns all created groups.
      operationId: GroupsGet
      x-api-path-slug: groups-get
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Groups
    post:
      summary: Create a new group
      description: Creates a new group in your license.
      operationId: GroupsPost
      x-api-path-slug: groups-post
      parameters:
      - in: formData
        name: agents[0]
      - in: formData
        name: agents[1]
      - in: formData
        name: name
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - New
      - Group
  /groups/{group_id}:
    get:
      summary: Get a single group details
      description: Returns group details for the given GROUP_ID.
      operationId: GroupsByGroupIdGet
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: path
        name: group_id
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Single
      - Group
      - Details
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