---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Fingerprint of Things Object Tagging Service List Groups
  description: List groups
  contact:
    name: NEC
  version: 1.0.0
host: fingerprint-of-things-ga1-dast.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/group/listGroups:
    post:
      summary: List Groups
      description: List groups
      operationId: groupReference
      x-api-path-slug: v1grouplistgroups-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
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