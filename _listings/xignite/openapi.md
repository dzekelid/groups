---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global Indices Real Time
  description: this-web-service-provides-global-real-time-information-for-u-s--and-international-indices-
  version: 1.0.0
host: globalindicesrealtime.xignite.com
basePath: xglobalindicesrealtime.json/XigniteGlobalIndicesRealTime
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListIndexGroups:
    get:
      summary: List Index Groups
      description: List index groups.
      operationId: ListIndexGroups
      x-api-path-slug: listindexgroups-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - List
      - Index
      - Groups
---