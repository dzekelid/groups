---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Create Group
  description: Used to create a group.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    post:
      summary: Create Group
      description: Used to create a group.
      operationId: createGroup
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
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