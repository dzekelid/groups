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
  /?Action=ModifyOptionGroup&k=1:
    get:
      summary: Modify Option Group
      description: Modifies an existing option group
      operationId: modifyoptiongroup
      parameters:
      - in: query
        name: ApplyImmediately
        description: Indicates whether the changes should be applied immediately,
          or during the next maintenance window for each instance associated with
          the option group
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be modified
        type: string
      - in: query
        name: OptionsToInclude.OptionConfiguration.N
        description: Options in this list are added to the option group or, if already
          present, the specified configuration is used to update the existing configuration
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: Options in this list are removed from the option group
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