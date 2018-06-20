---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Update Group
  version: 1.0.0
  description: Updates the specified group with the specified attributes.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AdminAddUserToGroup:
    get:
      summary: Admin Add User To Group
      description: Adds the specified user to the specified group.
      operationId: adminAddUserToGroup
      x-api-path-slug: actionadminaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminListGroupsForUser:
    get:
      summary: Admin List Groups For User
      description: Lists the groups that the user belongs to.
      operationId: adminListGroupsForUser
      x-api-path-slug: actionadminlistgroupsforuser-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=AdminRemoveUserFromGroup:
    get:
      summary: Admin Remove User From Group
      description: Removes the specified user from the specified group.
      operationId: adminRemoveUserFromGroup
      x-api-path-slug: actionadminremoveuserfromgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The group name
        type: string
      - in: query
        name: Username
        description: The username for the user
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=CreateGroup:
    get:
      summary: Create Group
      description: Creates a new group in the specified user pool.
      operationId: createGroup
      x-api-path-slug: actioncreategroup-get
      parameters:
      - in: query
        name: Description
        description: A string containing the description of the group
        type: string
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Precedence
        description: A nonnegative integer value that specifies the precedence of
          this group relative to            the other groups that a user can belong
          to in the user pool
        type: string
      - in: query
        name: RoleArn
        description: The role ARN for the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=DeleteGroup:
    get:
      summary: Delete Group
      description: Deletes a group.
      operationId: deleteGroup
      x-api-path-slug: actiondeletegroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=GetGroup:
    get:
      summary: Get Group
      description: Gets a group.
      operationId: getGroup
      x-api-path-slug: actiongetgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListGroups:
    get:
      summary: List Groups
      description: Lists the groups associated with a user pool.
      operationId: listGroups
      x-api-path-slug: actionlistgroups-get
      parameters:
      - in: query
        name: Limit
        description: The limit of the request to list groups
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListUsersInGroup:
    get:
      summary: List Users In Group
      description: Lists the users in the specified group.
      operationId: listUsersInGroup
      x-api-path-slug: actionlistusersingroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: NextToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /?Action=UpdateGroup:
    get:
      summary: Update Group
      description: Updates the specified group with the specified attributes.
      operationId: updateGroup
      x-api-path-slug: actionupdategroup-get
      parameters:
      - in: query
        name: Description
        description: A string containing the new description of the group
        type: string
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Precedence
        description: The new precedence value for the group
        type: string
      - in: query
        name: RoleArn
        description: The new role ARN for the group
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool
        type: string
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