---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API attribute group (2.x only)
  description: Attribute group (2.x only).
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/attribute-groups:
    get:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsGet
      x-api-path-slug: restv1attributegroups-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Groups
      - (2
      - X
      - Only)
    patch:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsPatch
      x-api-path-slug: restv1attributegroups-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Groups
      - (2
      - X
      - Only)
    post:
      summary: attribute group (2.x only)
      description: Assuming that there is no "new_attribute_group" already existing
      operationId: RestV1AttributeGroupsPost
      x-api-path-slug: restv1attributegroups-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
  /rest/v1/attribute-groups/technical:
    get:
      summary: attribute group (2.x only)
      description: Assuming that the given code is the code of an existing attribute
        group
      operationId: RestV1AttributeGroupsTechnicalGet
      x-api-path-slug: restv1attributegroupstechnical-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
    patch:
      summary: attribute group (2.x only)
      description: Attribute group (2.x only).
      operationId: RestV1AttributeGroupsTechnicalPatch
      x-api-path-slug: restv1attributegroupstechnical-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
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