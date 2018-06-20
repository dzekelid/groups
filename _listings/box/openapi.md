---
swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  description: the-box-content-api-gives-you-access-to-secure-content-management-and-content-experience-features-for-use-in-your-own-app--it-strives-to-be-restful-and-is-organized-around-the-main-resources-youre-familiar-with-from-the-box-web-interface-
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
---