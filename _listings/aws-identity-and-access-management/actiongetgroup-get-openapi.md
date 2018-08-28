---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Get Group
  version: 1.0.0
  description: Returns a list of IAM users that are in the specified IAM group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateGroup:
    get:
      summary: Create Group
      description: Creates a new group.
      operationId: createGroup
      x-api-path-slug: actioncreategroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to create
        type: string
      - in: query
        name: Path
        description: The path to the group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=DeleteGroup:
    get:
      summary: Delete Group
      description: Deletes the specified IAM group.
      operationId: deleteGroup
      x-api-path-slug: actiondeletegroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the IAM group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=GetGroup:
    get:
      summary: Get Group
      description: Returns a list of IAM users that are in the specified IAM group.
      operationId: getGroup
      x-api-path-slug: actiongetgroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListGroups:
    get:
      summary: List Groups
      description: Lists the IAM groups that have the specified path prefix.
      operationId: listGroups
      x-api-path-slug: actionlistgroups-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=UpdateGroup:
    get:
      summary: Update Group
      description: Updates the name and/or the path of the specified IAM group.
      operationId: updateGroup
      x-api-path-slug: actionupdategroup-get
      parameters:
      - in: query
        name: GroupName
        description: Name of the IAM group to update
        type: string
      - in: query
        name: NewGroupName
        description: New name for the IAM group
        type: string
      - in: query
        name: NewPath
        description: New path for the IAM group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
  /?Action=ListGroupsForUser:
    get:
      summary: List Groups For User
      description: Lists the IAM groups that the specified IAM user belongs to.
      operationId: listGroupsForUser
      x-api-path-slug: actionlistgroupsforuser-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the user to list groups for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups For User
  /?Action=AddUserToGroup:
    get:
      summary: Add User To Group
      description: Adds the specified user to the specified group.
      operationId: addUserToGroup
      x-api-path-slug: actionaddusertogroup-get
      parameters:
      - in: query
        name: GroupName
        description: The name of the group to update
        type: string
      - in: query
        name: UserName
        description: The name of the user to add
        type: string
      responses:
        200:
          description: OK
      tags:
      - User Groups
  /?Action=AttachGroupPolicy:
    get:
      summary: Attach Group Policy
      description: Attaches the specified managed policy to the specified IAM group.
      operationId: attachGroupPolicy
      x-api-path-slug: actionattachgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the group to attach the
          policy to
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          attach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=DeleteGroupPolicy:
    get:
      summary: Delete Group Policy
      description: |-
        Deletes the specified inline policy that is embedded in the specified IAM
              group.
      operationId: deleteGroupPolicy
      x-api-path-slug: actiondeletegrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) identifying the group that
          the policy is embedded      in
        type: string
      - in: query
        name: PolicyName
        description: The name identifying the policy document to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
  /?Action=DetachGroupPolicy:
    get:
      summary: Detach Group Policy
      description: Removes the specified managed policy from the specified IAM group.
      operationId: detachGroupPolicy
      x-api-path-slug: actiondetachgrouppolicy-get
      parameters:
      - in: query
        name: GroupName
        description: The name (friendly name, not ARN) of the IAM group to detach
          the policy      from
        type: string
      - in: query
        name: PolicyArn
        description: The Amazon Resource Name (ARN) of the IAM policy you want to
          detach
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group Policies
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