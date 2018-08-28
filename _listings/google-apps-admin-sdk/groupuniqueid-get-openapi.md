---
swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 0
info:
  title: Google Apps Admin SDK API Get Group
  version: 1.0.0
  description: Gets one resource by id.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{groupUniqueId}:
    get:
      summary: Get Group
      description: Gets one resource by id.
      operationId: groupsSettings.groups.get
      x-api-path-slug: groupuniqueid-get
      parameters:
      - in: path
        name: groupUniqueId
        description: The resource ID
      responses:
        200:
          description: OK
      tags:
      - Group
    patch:
      summary: Update Group
      description: Updates an existing resource. This method supports patch semantics.
      operationId: groupsSettings.groups.patch
      x-api-path-slug: groupuniqueid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupUniqueId
        description: The resource ID
      responses:
        200:
          description: OK
      tags:
      - Group
    put:
      summary: Update Group
      description: Updates an existing resource.
      operationId: groupsSettings.groups.update
      x-api-path-slug: groupuniqueid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupUniqueId
        description: The resource ID
      responses:
        200:
          description: OK
      tags:
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