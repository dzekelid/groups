swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
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
  /ListIndicesByIndexGroup:
    get:
      summary: List Indices By Index Group
      description: List indices by index group.
      operationId: ListIndicesByIndexGroup
      x-api-path-slug: listindicesbyindexgroup-get
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
      - Indices
      - Index
      - Group