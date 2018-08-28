swagger: "2.0"
x-collection-name: Gitter
x-complete: 1
info:
  title: Gitter
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: List Groups
      description: List groups the current user is in.
      operationId: listGroups
      x-api-path-slug: groups-get
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/:groupId/rooms:
    get:
      summary: Group Rooms
      description: List rooms under group
      operationId: getGroupRooms
      x-api-path-slug: groupsgroupidrooms-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Rooms