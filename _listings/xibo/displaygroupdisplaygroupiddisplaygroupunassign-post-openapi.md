---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Unassigns one or more DisplayGroups to a Display Group
  description: Removes the provided DisplayGroups from the Display Group
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup:
    get:
      summary: Get Display Groups
      description: ""
      operationId: displayGroupSearch
      x-api-path-slug: displaygroup-get
      parameters:
      - in: formData
        name: displayGroup
        description: Filter by DisplayGroup Name
      - in: formData
        name: displayGroupId
        description: Filter by DisplayGroup Id
      - in: formData
        name: displayId
        description: Filter by DisplayGroups containing a specific display
      - in: formData
        name: dynamicCriteria
        description: Filter by DisplayGroups containing a specific dynamic criteria
      - in: formData
        name: forSchedule
        description: Should the list be refined for only those groups the User can
          Schedule against?
      - in: formData
        name: isDisplaySpecific
        description: Filter by whether the Display Group belongs to a Display or is
          user created
      - in: formData
        name: nestedDisplayId
        description: Filter by DisplayGroups containing a specific display in there
          nesting
      responses:
        200:
          description: OK
      tags:
      - Display
      - Groups
    post:
      summary: Add a Display Group
      description: Add a new Display Group to the CMS
      operationId: displayGroupAdd
      x-api-path-slug: displaygroup-post
      parameters:
      - in: formData
        name: description
        description: The Display Group Description
      - in: formData
        name: displayGroup
        description: The Display Group Name
      - in: formData
        name: dynamicContent
        description: The filter criteria for this dynamic group
      - in: formData
        name: isDynamic
        description: Flag indicating whether this DisplayGroup is Dynamic
      - in: formData
        name: tags
        description: A comma separated list of tags for this item
      responses:
        200:
          description: OK
      tags:
      - Display
      - Group
  /displaygroup/{displayGroupId}:
    put:
      summary: Edit a Display Group
      description: Edit an existing Display Group identified by its Id
      operationId: displayGroupEdit
      x-api-path-slug: displaygroupdisplaygroupid-put
      parameters:
      - in: formData
        name: description
        description: The Display Group Description
      - in: formData
        name: displayGroup
        description: The Display Group Name
      - in: path
        name: displayGroupId
        description: The displayGroupId to edit
      - in: formData
        name: dynamicCriteria
        description: The filter criteria for this dynamic group
      - in: formData
        name: isDynamic
        description: Flag indicating whether this DisplayGroup is Dynamic
      - in: formData
        name: tags
        description: A comma separated list of tags for this item
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Display
      - Group
    delete:
      summary: Delete a Display Group
      description: Delete an existing Display Group identified by its Id
      operationId: displayGroupDelete
      x-api-path-slug: displaygroupdisplaygroupid-delete
      parameters:
      - in: path
        name: displayGroupId
        description: The displayGroupId to delete
      responses:
        200:
          description: OK
      tags:
      - Display
      - Group
  /displaygroup/{displayGroupId}/display/assign:
    post:
      summary: Assign one or more Displays to a Display Group
      description: Adds the provided Displays to the Display Group
      operationId: displayGroupDisplayAssign
      x-api-path-slug: displaygroupdisplaygroupiddisplayassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: displayId
        description: The Display Ids to assign
      - in: formData
        name: unassignDisplayId
        description: An optional array of Display IDs to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - Displays
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/display/unassign:
    post:
      summary: Unassigns one or more Displays to a Display Group
      description: Removes the provided Displays from the Display Group
      operationId: displayGroupDisplayUnassign
      x-api-path-slug: displaygroupdisplaygroupiddisplayunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: displayId
        description: The Display Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassigns
      - More
      - Displays
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/displayGroup/assign:
    post:
      summary: Assign one or more DisplayGroups to a Display Group
      description: Adds the provided DisplayGroups to the Display Group
      operationId: displayGroupDisplayGroupAssign
      x-api-path-slug: displaygroupdisplaygroupiddisplaygroupassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: displayGroupId
        description: The displayGroup Ids to assign
      - in: formData
        name: unassignDisplayGroupId
        description: An optional array of displayGroup IDs to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - DisplayGroups
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/displayGroup/unassign:
    post:
      summary: Unassigns one or more DisplayGroups to a Display Group
      description: Removes the provided DisplayGroups from the Display Group
      operationId: displayGroupDisplayGroupUnassign
      x-api-path-slug: displaygroupdisplaygroupiddisplaygroupunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: displayGroupId
        description: The DisplayGroup Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassigns
      - More
      - DisplayGroups
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/media/assign:
    post:
      summary: Assign one or more Media items to a Display Group
      description: Adds the provided Media to the Display Group
      operationId: displayGroupMediaAssign
      x-api-path-slug: displaygroupdisplaygroupidmediaassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: mediaId
        description: The Media Ids to assign
      - in: formData
        name: unassignMediaId
        description: Optional array of Media Id to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - Media
      - Items
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/media/unassign:
    post:
      summary: Unassign one or more Media items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupMediaUnassign
      x-api-path-slug: displaygroupdisplaygroupidmediaunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: mediaId
        description: The Media Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Media
      - Items
      - From
      - Display
      - Group
  /displaygroup/{displayGroupId}/layout/assign:
    post:
      summary: Assign one or more Layouts items to a Display Group
      description: Adds the provided Layouts to the Display Group
      operationId: displayGroupLayoutsAssign
      x-api-path-slug: displaygroupdisplaygroupidlayoutassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to assign to
      - in: formData
        name: layoutId
        description: The Layouts Ids to assign
      - in: formData
        name: unassignLayoutId
        description: Optional array of Layouts Id to unassign
      responses:
        200:
          description: OK
      tags:
      - Assign
      - More
      - Layouts
      - Items
      - To
      - Display
      - Group
  /displaygroup/{displayGroupId}/layout/unassign:
    post:
      summary: Unassign one or more Layout items from a Display Group
      description: Removes the provided from the Display Group
      operationId: displayGroupLayoutUnassign
      x-api-path-slug: displaygroupdisplaygroupidlayoutunassign-post
      parameters:
      - in: path
        name: displayGroupId
        description: The Display Group to unassign from
      - in: formData
        name: layoutId
        description: The Layout Ids to unassign
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - More
      - Layout
      - Items
      - From
      - Display
      - Group
  /group/{userGroupId}/copy:
    post:
      summary: Copy User Group
      description: Copy an user group, optionally copying the group members
      operationId: userGroupCopy
      x-api-path-slug: groupusergroupidcopy-post
      parameters:
      - in: formData
        name: copyMembers
        description: Flag indicating whether to copy group members
      - in: formData
        name: group
        description: The Group Name
      - in: path
        name: userGroupId
        description: The User Group ID to Copy
      responses:
        200:
          description: OK
      tags:
      - Copy
      - User
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