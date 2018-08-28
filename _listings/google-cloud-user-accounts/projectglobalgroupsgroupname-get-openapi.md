---
swagger: "2.0"
x-collection-name: Google Cloud User Accounts
x-complete: 0
info:
  title: Google Cloud User Accounts API Get Group
  description: Returns the specified Group resource.
  contact:
    name: Google
    url: https://google.com
  version: vm_alpha
host: www.googleapis.com
basePath: /clouduseraccounts/vm_alpha/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/groups:
    get:
      summary: Get Groups
      description: Retrieves the list of groups contained within the specified project.
      operationId: clouduseraccounts.groups.list
      x-api-path-slug: projectglobalgroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    post:
      summary: Create Group
      description: Creates a Group resource in the specified project using the data
        included in the request.
      operationId: clouduseraccounts.groups.insert
      x-api-path-slug: projectglobalgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
  /{project}/global/groups/{groupName}:
    delete:
      summary: Delete Group
      description: Deletes the specified Group resource.
      operationId: clouduseraccounts.groups.delete
      x-api-path-slug: projectglobalgroupsgroupname-delete
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Group
    get:
      summary: Get Group
      description: Returns the specified Group resource.
      operationId: clouduseraccounts.groups.get
      x-api-path-slug: projectglobalgroupsgroupname-get
      parameters:
      - in: path
        name: groupName
        description: Name of the Group resource to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
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