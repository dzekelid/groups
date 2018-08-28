---
swagger: "2.0"
x-collection-name: Vestorly
x-complete: 0
info:
  title: Vestorly Put Groups
  description: Updates a Group
  termsOfService: http://www.vestorly.com/terms/
  contact:
    name: Vestorly Team
  version: 1.0.0
host: staging.vestorly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: Get Groups
      description: Returns all groups
      operationId: findGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Post Groups
      description: Creates a new Group
      operationId: createGroup
      x-api-path-slug: groups-post
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: group
        description: Group to add
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{id}:
    delete:
      summary: Delete Groups
      description: Deletes a Group
      operationId: deleteGroup
      x-api-path-slug: groupsid-delete
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: id of group to delete
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Returns a single group if user has access
      operationId: findGroupByID
      x-api-path-slug: groupsid-get
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: path
        name: id
        description: Mongo ID of group to fetch
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Put Groups
      description: Updates a Group
      operationId: updateGroupById
      x-api-path-slug: groupsid-put
      parameters:
      - in: query
        name: access_token
        description: OAuth Token
      - in: body
        name: group
        description: Group to update
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of group to update
      - in: query
        name: vestorly-auth
        description: Vestorly Auth Token
      - in: query
        name: vestorly_auth
        description: Vestorly Auth Token
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