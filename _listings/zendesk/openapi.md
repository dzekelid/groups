---
swagger: "2.0"
x-collection-name: Zendesk
x-complete: 1
info:
  title: Sales Force Desk API
  description: build-deep-integrations-expose-your-service-to-influential-smb-customers-or-just-make-desk-com-work-the-way-you-want-
  version: v2
host: yoursite.desk.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups.{format}:
    get:
      summary: Get Groups
      description: Get groups.
      operationId: get-groups
      x-api-path-slug: groups-format-get
      parameters:
      - in: path
        name: format
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Format
  /groups/{id}.{format}:
    get:
      summary: Get Group
      description: Get group.
      operationId: get-group
      x-api-path-slug: groupsid-format-get
      parameters:
      - in: path
        name: format
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Format
---