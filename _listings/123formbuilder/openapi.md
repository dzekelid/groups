swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: Get all user groups
      description: Get all user groups
      operationId: get-all-user-groups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of groups to get per page in a request
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
    post:
      summary: Create a new group
      description: Create a new group
      operationId: create-a-new-group
      x-api-path-slug: groups-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: Form name
      - in: formData
        name: parent_id
        description: Indicates the ID of the parent group
      - in: formData
        name: webhook_url
        description: The URL of the WebHook
      responses:
        200:
          description: OK
      tags:
      - New
      - Group
  /groups/{group_id}:
    get:
      summary: Get group details
      description: Get information about a specific group.
      operationId: get-information-about-a-specific-group
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: path
        name: group_id
        description: The ID of the group
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Group
      - Details
    put:
      summary: Update group data
      description: Updates the details of a group.
      operationId: updates-the-details-of-a-group
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to edit
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: This is required when the webhook_url or parent_id is missing
      - in: formData
        name: parent_id
        description: Indicates the ID of the parent group
      - in: formData
        name: webhook_url
        description: This is required when the name or parent_id is missing
      responses:
        200:
          description: OK
      tags:
      - Group
      - Data
  /groups/{group_id}/forms:
    get:
      summary: Get all forms in a group
      description: Displays a list of all of the forms within a specific group.
      operationId: displays-a-list-of-all-of-the-forms-within-a-specific-group
      x-api-path-slug: groupsgroup-idforms-get
      parameters:
      - in: path
        name: group_id
        description: The ID of the group
      - in: query
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Forms
      - In
      - Group
  /groups/{group_id}/share:
    post:
      summary: Share a group with a user
      description: This may not be available for your account. It is specific to certain
        users.
      operationId: this-may-not-be-available-for-your-account-it-is-specific-to-certain-users
      x-api-path-slug: groupsgroup-idshare-post
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to share
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: subuser_email
        description: The username with whom you want to share this group
      - in: formData
        name: subuser_id
        description: The ID of the user with whom you want to share this group
      responses:
        200:
          description: OK
      tags:
      - Share
      - Group
      - User
  /groups/{group_id}/unshare:
    post:
      summary: Unshare a group from a user
      description: This may not be available for your account. It is specific to certain
        users.
      operationId: this-may-not-be-available-for-your-account-it-is-specific-to-certain-users
      x-api-path-slug: groupsgroup-idunshare-post
      parameters:
      - in: path
        name: group_id
        description: The ID of the group you want to unshare
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: subuser_email
        description: The username from whom you want to unshare the group
      - in: formData
        name: subuser_id
        description: The ID of the subuser from whom you want to unshare the group
      responses:
        200:
          description: OK
      tags:
      - Unshare
      - Group
      - From
      - User