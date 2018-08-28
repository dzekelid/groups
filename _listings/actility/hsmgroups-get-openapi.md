---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Maker API HSM groups retrieval
  description: Retrieves all HSM groups.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hsmGroups:
    get:
      summary: HSM groups retrieval
      description: Retrieves all HSM groups.
      operationId: retrieves-all-hsm-groups
      x-api-path-slug: hsmgroups-get
      parameters:
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 HSM groups
          of the specified page
      responses:
        200:
          description: OK
      tags:
      - HSM
      - Groups
      - Retrieval
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