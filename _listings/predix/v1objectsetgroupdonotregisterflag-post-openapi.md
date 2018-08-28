---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Fingerprint of Things Object Tagging Service Switch Apply Flag per
    Group
  description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag per
    group'
  contact:
    name: NEC
  version: 1.0.0
host: fingerprint-of-things-ga1-dast.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/group/listGroups:
    post:
      summary: List Groups
      description: List groups
      operationId: groupReference
      x-api-path-slug: v1grouplistgroups-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
  /v1/group/createGroup:
    post:
      summary: Create Group
      description: Create group.
      operationId: createGroup
      x-api-path-slug: v1groupcreategroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Group
  /v1/group/deleteGroup:
    post:
      summary: Delete Group
      description: Delete group.
      operationId: deleteGroup
      x-api-path-slug: v1groupdeletegroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Group
  /v1/object/setGroupDoNotRegisterFlag:
    post:
      summary: Switch Apply Flag per Group
      description: '* DO NOT USE. This API will be deleted.<br>Switch the Apply flag
        per group'
      operationId: groupConfig
      x-api-path-slug: v1objectsetgroupdonotregisterflag-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Switch
      - Apply
      - Flag
      - Per
      - Group
  /v1/group/putInGroup:
    post:
      summary: Put Object in Group
      description: Put Object in Group.
      operationId: joinGroup
      x-api-path-slug: v1groupputingroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Object
      - In
      - Group
  /v1/group/removeFromGroup:
    post:
      summary: Remove Object from Group
      description: Remove Object from Group.
      operationId: leaveGroup
      x-api-path-slug: v1groupremovefromgroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Object
      - From
      - Group
  /v1/object/registerGroup:
    post:
      summary: Register Object per Group
      description: Register Object per Group. A registered object can be queried from
        Query APIs.
      operationId: groupApply
      x-api-path-slug: v1objectregistergroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
      - Per
      - Group
  /v1/query/queryByGroup:
    post:
      summary: Query by Group
      description: Query image per group.
      operationId: groupzicheck
      x-api-path-slug: v1queryquerybygroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: formData
        name: checkResultDisplayNumber
        description: 'Result display number: Specify number of verification result
          to retrieve'
      - in: formData
        name: groupId
        description: 'Group ID: Use CSV form when specifying multiple IDs'
      - in: formData
        name: idSpecificationFlag
        description: 'ID specification flag(0: Query with all registered objects ,
          1: Query with specified object by groupId)'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      - in: formData
        name: queryImage
        description: 'Query image data(Max file size: 5MByte)'
      responses:
        200:
          description: OK
      tags:
      - Query
      - By
      - Group
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