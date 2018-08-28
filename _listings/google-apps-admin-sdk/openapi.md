swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
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