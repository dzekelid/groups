---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API Delete Group
  version: 1.0.0
  description: Deletes the specified IAM group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteGroup:
    get:
      summary: ' Delete Group '
      description: Deletes the specified IAM group
      operationId: deleteGroup
      parameters:
      - in: query
        name: GroupName
        description: The name of the IAM group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - groups
definitions: []
x-collection-name: AWS Identity and Access Management
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