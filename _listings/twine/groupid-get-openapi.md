---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get a group
  description: Get a group record by id.
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /group:
    get:
      summary: List groups
      description: Get a list of groups matching the specified filters.
      operationId: fetchGroups
      x-api-path-slug: group-get
      parameters:
      - in: query
        name: filter[name]
        description: Group name
      - in: query
        name: filter[organization]
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groups
    post:
      summary: Create a group
      description: Create a group record.
      operationId: createGroup
      x-api-path-slug: group-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Group
  /group/{id}:
    get:
      summary: Get a group
      description: Get a group record by id.
      operationId: fetchGroup
      x-api-path-slug: groupid-get
      parameters:
      - in: path
        name: id
        description: Group identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Group
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