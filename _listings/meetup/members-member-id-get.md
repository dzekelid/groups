---
swagger: "2.0"
info:
  title: Meetup Get Member Profile
  description: |-
    Gets Member Profiles.
    For Group Profiles, see [this endpoint](/meetup_api/docs/:urlname/members/:member_id)
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/:member_id:
    get:
      summary: Get Member Profile
      description: Gets Member Profiles
      operationId: profiles
      parameters:
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - groups
definitions: []
x-collection-name: Meetup
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