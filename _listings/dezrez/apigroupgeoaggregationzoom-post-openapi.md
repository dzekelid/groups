---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Returns GeoAggregations of all searching groups
  version: 1.0.0
  description: Returns geoaggregations of all searching groups.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/setbranch:
    post:
      summary: Set the Groups home Branch
      description: Set the groups home branch.
      operationId: Group_SetBranchByidBysetBranchCommand
      x-api-path-slug: apigroupidsetbranch-post
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setBranchCommand
        description: The set branch data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Groups
      - Home
      - Branch
  /api/group/{id}/setteam:
    post:
      summary: Set the Groups owning team
      description: Set the groups owning team.
      operationId: Group_SetOwningTeamByidBysetTeamCommand
      x-api-path-slug: apigroupidsetteam-post
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setTeamCommand
        description: The set owning team data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Groups
      - Owning
      - Team
  /api/group/updateprimarygroupmember:
    put:
      summary: Return the Groups with appointments between a given date range, ordered
        by appointments Count
      description: Return the groups with appointments between a given date range,
        ordered by appointments count.
      operationId: Group_UpdatePrimaryGroupMemberByfilter
      x-api-path-slug: apigroupupdateprimarygroupmember-put
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Appointments
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Appointments
      - Count
  /api/group/mostactive:
    get:
      summary: Return the Groups with the most viewings between a given date range,
        ordered by viewing Count
      description: Return the groups with the most viewings between a given date range,
        ordered by viewing count.
      operationId: Group_MostActiveBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.roleTypes
      x-api-path-slug: apigroupmostactive-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Most
      - Viewings
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Viewing
      - Count
  /api/group/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all searching groups
      description: Returns geoaggregations of all searching groups.
      operationId: Group_GeoAggregationByzoom
      x-api-path-slug: apigroupgeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Searching
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