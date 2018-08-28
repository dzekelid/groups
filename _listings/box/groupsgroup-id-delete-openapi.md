---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Delete Group
  description: Permanently deletes a specific group.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    post:
      summary: Create Group
      description: Used to create a group.
      operationId: createGroup
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
    get:
      summary: Get Groups for an Enterprise
      description: Retrieves all of the groups for given enterprise. Must have permissions
        to see an enterprise's groups.
      operationId: getEnterpriseGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
  /groups/{GROUP_ID}:
    get:
      summary: Get Group
      description: Used to get information about a group.
      operationId: getGroup
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
    put:
      summary: Update Group
      description: Updates a specific group.
      operationId: updateGroup
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
    delete:
      summary: Delete Group
      description: Permanently deletes a specific group.
      operationId: deleteGroup
      x-api-path-slug: groupsgroup-id-delete
      parameters:
      - in: path
        name: GROUP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
  /groups/{GROUP_ID}/memberships:
    get:
      summary: Get Memberships for Group
      description: Retrieves all of the members for a given group if the requesting
        user has access (see Group Object member_viewability_level).
      operationId: getGroupMemberships
      x-api-path-slug: groupsgroup-idmemberships-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_ID
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
      - ""
      - Memberships
  /groups/{GROUP_ID}/collaborations:
    get:
      summary: Get Collaborations for Group
      description: Retrieves all of the group collaborations for a given group. Note
        this is only available to group admins.
      operationId: getGroupCollaborations
      x-api-path-slug: groupsgroup-idcollaborations-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_ID
      - in: query
        name: limit
        description: The maximum number of items to return in a page
      - in: query
        name: offset
        description: The item at which to begin the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Groups
      - Group
      - ""
      - Collaborations
  /group_memberships:
    post:
      summary: Create Membership
      description: Used to add a member to a Group.
      operationId: createGroupMembership
      x-api-path-slug: group-memberships-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
  /group_memberships/{GROUP_MEMBERSHIP_ID}:
    get:
      summary: Get Membership
      description: Fetches a specific group membership entry.
      operationId: getGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-get
      parameters:
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_MEMBERSHIP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
      - Group
      - Membership
    put:
      summary: Update Membership
      description: Used to update a group membership.
      operationId: updateGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: GROUP_MEMBERSHIP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
      - Group
      - Membership
    delete:
      summary: Delete Membership
      description: Deletes a specific group membership.
      operationId: deleteGroupMembership
      x-api-path-slug: group-membershipsgroup-membership-id-delete
      parameters:
      - in: path
        name: GROUP_MEMBERSHIP_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Group
      - Memberships
      - Group
      - Membership
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