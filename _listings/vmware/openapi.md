swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /internal/resources/groups:
    get:
      summary: Get Custom Groups
      description: 'TODO: Add Description'
      operationId: InternalResourcesGroupsGet
      x-api-path-slug: internalresourcesgroups-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Resources
      - Groups
    post:
      summary: Create Custom Group
      description: 'TODO: Add Description'
      operationId: InternalResourcesGroupsPost
      x-api-path-slug: internalresourcesgroups-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Resources
      - Groups