---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Get Group
  description: |-
    Returns a group or multiple groups by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/groups:
    get:
      summary: Get User Groups
      description: |-
        Returns the list of groups associated with the user.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: listGlipGroups
      x-api-path-slug: restapiv1-0glipgroups-get
      parameters:
      - in: query
        name: pageToken
        description: Token of a page to be returned
      - in: query
        name: recordCount
        description: Max numbers of records to be returned
      - in: query
        name: type
        description: Type of a group
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
    post:
      summary: Create Group
      description: |-
        Creates a group.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: createGlipGroup
      x-api-path-slug: restapiv1-0glipgroups-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Group
  /restapi/v1.0/account/{accountId}/call-monitoring-groups:
    get:
      summary: Get Call Monitoring Groups
      description: |-
        Returns call monitoring groups that can be filtered by some extension.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallMonitoringGroups
      x-api-path-slug: restapiv1-0accountaccountidcallmonitoringgroups-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: memberExtensionId
        description: Internal identifier of an extension that is a member of every
          group within the result
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Monitoring
      - Groups
  /restapi/v1.0/glip/groups/{groupId}:
    get:
      summary: Get Group
      description: |-
        Returns a group or multiple groups by their ID(s). Batch request is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipGroup
      x-api-path-slug: restapiv1-0glipgroupsgroupid-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group to be returned, the maximum number
          of IDs is 30
      responses:
        200:
          description: OK
      tags:
      - Group
  /restapi/v1.0/glip/groups/{groupId}/bulk-assign:
    post:
      summary: Edit Group Members
      description: |-
        Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: assignGlipGroupMembers
      x-api-path-slug: restapiv1-0glipgroupsgroupidbulkassign-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Group
      - Members
  /restapi/v1.0/glip/groups/{groupId}/posts:
    get:
      summary: Get Group Posts
      description: |-
        Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
        Usage Plan Group
        Medium
      operationId: listGlipGroupPosts
      x-api-path-slug: restapiv1-0glipgroupsgroupidposts-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group
      - in: query
        name: pageToken
        description: Pagination token
      - in: query
        name: recordCount
        description: Max number of records to be returned
      responses:
        200:
          description: OK
      tags:
      - Group
      - S
    post:
      summary: Create Post in Group
      description: |-
        Creates a new post in a group specified.
        Usage Plan Group
        Medium
      operationId: createGlipGroupPost
      x-api-path-slug: restapiv1-0glipgroupsgroupidposts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - In
      - Group
  /restapi/v1.0/glip/groups/{groupId}/webhooks:
    post:
      summary: Create Webhook in Group
      description: |-
        Create new Webhook
        Usage Plan Group
        Medium
      operationId: createGlipGroupWebhook
      x-api-path-slug: restapiv1-0glipgroupsgroupidwebhooks-post
      parameters:
      - in: path
        name: groupId
        description: Group id
      responses:
        200:
          description: OK
      tags:
      - Webhook
      - In
      - Group
    get:
      summary: Get Webhooks in Group
      description: |-
        Returns webhooks which are available for the current user (by group ID).
        Usage Plan Group
        Medium
      operationId: listGlipGroupWebhooks
      x-api-path-slug: restapiv1-0glipgroupsgroupidwebhooks-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - In
      - Group
  /restapi/v1.0/account/{accountId}/paging-only-groups/{pagingOnlyGroupId}/users:
    get:
      summary: Get Paging Only Group Users
      description: "Returns the list of users allowed to page this group.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadAccounts]
        permission"
      operationId: listPagingGroupUsers
      x-api-path-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: path
        name: pagingOnlyGroupId
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Paging
      - Only
      - Group
      - Users
  /restapi/v1.0/account/{accountId}/paging-only-groups/{pagingOnlyGroupId}/devices:
    get:
      summary: Get Paging Only Group Devices
      description: "Returns the list of paging devices assigned to this group.\nApp
        Permission\nReadAccounts\nUser Permission\nReadCompanyDevices\nUsage Plan
        Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadAccounts] permission"
      operationId: listPagingGroupDevices
      x-api-path-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: path
        name: pagingOnlyGroupId
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Paging
      - Only
      - Group
      - Devices
  /restapi/v1.0/account/{accountId}/paging-only-groups/{pagingOnlyGroupId}/bulk-assign:
    post:
      summary: Edit Paging Group Users and Devices
      description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
        Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [addedDeviceIds] value is invalid\n\n\n403\nCMN-401\nIn order to call this
        API endpoint, application needs to have [EditAccounts] permission"
      operationId: bulkAssignPagingGroup
      x-api-path-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pagingOnlyGroupId
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Paging
      - Group
      - Users
      - Devices
  /restapi/v1.0/account/{accountId}/call-queues/{groupId}/bulk-assign:
    post:
      summary: Edit Call Queue Group
      description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser
        Permission\nGroups\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n400\nEXT-405\nExtension of
        type [ParkLocation] could not be a member of [department}]"
      operationId: updateCallQueueGroup
      x-api-path-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        description: Changes for the given group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Call
      - Queue
      - Group
  /restapi/v1.0/account/{accountId}/call-monitoring-groups/{groupId}/members:
    get:
      summary: Get Call Monitoring Group Members
      description: |-
        Returns call monitoring group members.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallMonitoringGroupMembers
      x-api-path-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: groupId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Monitoring
      - Group
      - Members
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