---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Group Get Member Groups
  description: 'group: getMemberGroups Return all the groups that the specified group
    is a member of. The check is transitive, unlike reading the memberOf navigation
    property, which returns only the groups that the group is a direct member of.'
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/checkMemberGroups:
    post:
      summary: Check Member Groups
      description: Check member groups Check for membership in a specified list of
        groups, and returns from that list those groups of which the specified user,
        group, or directory object is a member. This function is transitive.
      operationId: CheckMemberGroups
      x-api-path-slug: mecheckmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Member
      - Groups
  /users/{id | userPrincipalName}/checkMemberGroups:
    post:
      summary: Check Member Groups
      description: Check member groups Check for membership in a specified list of
        groups, and returns from that list those groups of which the specified user,
        group, or directory object is a member. This function is transitive.
      operationId: CheckMemberGroups
      x-api-path-slug: usersid--userprincipalnamecheckmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Member
      - Groups
  /groups/{id}/checkMemberGroups:
    post:
      summary: Group Check Member Groups
      description: 'group: checkMemberGroups Check for membership in the specified
        list of groups. Returns from the list those groups of which the specified
        group has a direct or transitive membership.'
      operationId: Group:CheckMemberGroups
      x-api-path-slug: groupsidcheckmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Checks
      - Member
      - Groups
  /directoryObjects/{id}/checkMemberGroups:
    post:
      summary: Check Member Groups
      description: Check member groups Check for membership in a specified list of
        groups, and returns from that list those groups of which the specified user,
        group, or directory object is a member. This function is transitive.
      operationId: CheckMemberGroups
      x-api-path-slug: directoryobjectsidcheckmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Member
      - Groups
  /me/getMemberGroups:
    post:
      summary: Get Member Groups
      description: Get member groups Return all the groups that the specified user,
        group, or directory object is a member of. This function is transitive.
      operationId: GetMemberGroups
      x-api-path-slug: megetmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      responses:
        200:
          description: OK
      tags:
      - Member
      - Groups
  /users/{id | userPrincipalName}/getMemberGroups:
    post:
      summary: Get Member Groups
      description: Get member groups Return all the groups that the specified user,
        group, or directory object is a member of. This function is transitive.
      operationId: GetMemberGroups
      x-api-path-slug: usersid--userprincipalnamegetmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Member
      - Groups
  /groups/{id}/getMemberGroups:
    post:
      summary: Group Get Member Groups
      description: 'group: getMemberGroups Return all the groups that the specified
        group is a member of. The check is transitive, unlike reading the memberOf
        navigation property, which returns only the groups that the group is a direct
        member of.'
      operationId: Group:GetMemberGroups
      x-api-path-slug: groupsidgetmembergroups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        type: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - ""
      - Member
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