---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CopyDBParameterGroup&k=1:
    get:
      summary: Copy D B Parameter Group
      description: Copies the specified DB parameter group
      operationId: copydbparametergroup
      parameters:
      - in: query
        name: SourceDBParameterGroupIdentifier
        description: The identifier or ARN for the source DB parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBParameterGroupDescription
        description: A description for the copied DB parameter group
        type: string
      - in: query
        name: TargetDBParameterGroupIdentifier
        description: The identifier for the copied DB parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - parameter groups
definitions: []
x-collection-name: AWS RDS
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