---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Add user to a user group by user name
  version: 1.0.0
  description: Add user to a user group by user name.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/groups/{groupid}:
    put:
      summary: Add user to a user group by user id
      description: Add user to a user group by user id.
      operationId: addUserToGroupByUserid
      x-api-path-slug: usersuseridgroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - User
      - Group
      - By
      - User
  /users/{userid}/groups:
    get:
      summary: Gets a user's group list by user id
      description: Gets a user's group list by user id.
      operationId: getUserGroupsByUserid
      x-api-path-slug: usersuseridgroups-get
      parameters:
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Group
      - List
      - By
      - User
  /users/myself/groups/{groupid}:
    put:
      summary: Add current user to a user group
      description: Add current user to a user group.
      operationId: addMyselfToGroup
      x-api-path-slug: usersmyselfgroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - To
      - User
      - Group
  /users/myself/groups:
    get:
      summary: Gets current user's group list
      description: Gets current user's group list.
      operationId: getMyUserGroups
      x-api-path-slug: usersmyselfgroups-get
      responses:
        200:
          description: OK
      tags:
      - Current
      - Users
      - Group
      - List
  /users/by-username/{username}/groups/{groupid}:
    put:
      summary: Add user to a user group by user name
      description: Add user to a user group by user name.
      operationId: addUserToGroupByUsername
      x-api-path-slug: usersbyusernameusernamegroupsgroupid-put
      parameters:
      - in: path
        name: groupid
        description: Group id
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - User
      - Group
      - By
      - User
      - Name
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