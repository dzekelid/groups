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
  /?Action=DescribeOptionGroups&k=1:
    get:
      summary: Describe Option Groups
      description: Describes the available option groups
      operationId: describeoptiongroups
      parameters:
      - in: query
        name: EngineName
        description: Filters the list of option groups to only include groups associated
          with a specific database engine
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: MajorEngineVersion
        description: Filters the list of option groups to only include groups associated
          with a specific database engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeOptionGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to describe
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