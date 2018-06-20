---
swagger: "2.0"
x-collection-name: Apica
x-complete: 0
info:
  title: Groups API Groups
  version: 1.0.0
  description: Gets a hierarchy of all monitor groups that are visible to you as a
    user or a customer depending on the request context.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/groups ':
    ' get ':
      summary: Groups
      description: Gets a hierarchy of all monitor groups that are visible to you
        as a user or a customer depending on the request context.
      operationId: -groups-
      x-api-path-slug: groups-get
      responses:
        200:
          description: OK
      tags:
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