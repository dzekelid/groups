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
  /?Action=CreateOptionGroup&k=1:
    get:
      summary: Create Option Group
      description: Creates a new option group
      operationId: createoptiongroup
      parameters:
      - in: query
        name: EngineName
        description: Specifies the name of the engine that this option group should
          be associated with
        type: string
      - in: query
        name: MajorEngineVersion
        description: Specifies the major version of the engine that this option group
          should be associated with
        type: string
      - in: query
        name: OptionGroupDescription
        description: The description of the option group
        type: string
      - in: query
        name: OptionGroupName
        description: Specifies the name of the option group to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - option groups
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