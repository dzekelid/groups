---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get User Groups
  description: |-
    Returns the list of groups associated with the user.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/groups:
    get:
      summary: Get User Groups
      description: |-
        Returns the list of groups associated with the user.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: listGlipGroups
      x-api-path-slug: restapiv1-0glipgroups-get
      parameters:
      - in: query
        name: pageToken
        description: Token of a page to be returned
      - in: query
        name: recordCount
        description: Max numbers of records to be returned
      - in: query
        name: type
        description: Type of a group
      responses:
        200:
          description: OK
      tags:
      - User
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