---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get user groups
  description: Returns the groups to which a user belongs. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Browse users and groups_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /group:
    get:
      summary: Get groups
      description: |-
        Returns all user groups. The returned groups are ordered alphabetically in
        ascending order by group name.

        **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
        Permission to access the Confluence site ('Can use' global permission).
      operationId: com.atlassian.confluence.plugins.restapi.resources.GroupResource.getGroups_get
      x-api-path-slug: group-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of groups to return per page
      - in: query
        name: start
        description: The starting index of the returned groups
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
        200:
          description: OK
      tags:
      - Groups
  /content/{id}/restriction/byOperation/{operationKey}/group/{groupName}:
    put:
      summary: Add group to content restriction
      description: "Adds a group to a content restriction. That is, grant read or
        update \npermission to the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to edit the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentRestrictionResource.addGroupToContentRestr
      x-api-path-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-put
      parameters:
      - in: path
        name: groupName
        description: The name of the group to add to the content restriction
      - in: path
        name: id
        description: The ID of the content that the restriction applies to
      - in: path
        name: operationKey
        description: The operation that the restriction applies to
      responses:
        200:
          description: OK
      tags:
      - Group
      - To
      - Content
      - Restriction
    delete:
      summary: Remove group from content restriction
      description: "Removes a group from a content restriction. That is, remove read
        or update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to edit the content."
      operationId: com.atlassian.confluence.plugins.restapi.resources.ContentRestrictionResource.removeGroupFromContent
      x-api-path-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-delete
      parameters:
      - in: path
        name: groupName
        description: The name of the group to remove from the content restriction
      - in: path
        name: id
        description: The ID of the content that the restriction applies to
      - in: path
        name: operationKey
        description: The operation that the restriction applies to
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Content
      - Restriction
  /group/{groupName}:
    get:
      summary: Get group
      description: |-
        Returns a user group for a given group name.

        **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
        Permission to access the Confluence site ('Can use' global permission).
      operationId: com.atlassian.confluence.plugins.restapi.resources.GroupResource.getGroup_get
      x-api-path-slug: groupgroupname-get
      parameters:
      - in: path
        name: groupName
        description: The name of the group
      responses:
        200:
          description: OK
      tags:
      - Group
  /group/{groupName}/member:
    get:
      summary: Get group members
      description: |-
        Returns the users that are members of a group.

        **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
        Permission to access the Confluence site ('Can use' global permission).
      operationId: com.atlassian.confluence.plugins.restapi.resources.GroupResource.getGroupMembers_get
      x-api-path-slug: groupgroupnamemember-get
      parameters:
      - in: path
        name: groupName
        description: The name of the group to be queried for its members
      - in: query
        name: limit
        description: The maximum number of users to return per page
      - in: query
        name: start
        description: The starting index of the returned users
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members
  /user/memberof:
    get:
      summary: Get group memberships for user
      description: "Returns the groups that a user is a member of.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to access the Confluence site ('Can use' global permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserResource.getGroupMembershipsForUser_get
      x-api-path-slug: usermemberof-get
      parameters:
      - in: query
        name: accountId
        description: The accountId of the user to be queried
      - in: query
        name: key
        description: The userKey of the user to be queried
      - in: query
        name: limit
        description: The maximum number of groups to return per page
      - in: query
        name: start
        description: The starting index of the returned groups
      - in: query
        name: username
        description: The username of the user to be queried
      responses:
        200:
          description: OK
      tags:
      - Group
      - Membershipsuser
  /api/2/groups/picker:
    get:
      summary: Find groups
      description: |-
        Returns groups with substrings matching a given query. This is mainly for use with the group picker, so the returned groups contain html to be used as picker suggestions. The groups are also wrapped in a single response object that also contains a header for use in the picker, specifically _Showing X of Y matching groups_.

        The number of groups returned is limited by the system property "jira.ajax.autocomplete.limit"

        The groups will be unique and sorted.
      operationId: com.atlassian.jira.rest.v2.issue.GroupPickerResource.findGroups_get
      x-api-path-slug: api2groupspicker-get
      parameters:
      - in: query
        name: accountId
      - in: query
        name: exclude
      - in: header
        name: force-account-id
      - in: query
        name: maxResults
      - in: query
        name: query
        description: a String to match groups agains
      - in: query
        name: userName
      responses:
        200:
          description: OK
      tags:
      - Find
      - Groups
  /api/2/groupuserpicker:
    get:
      summary: Find users and groups
      description: Returns a list of users and groups matching query with highlighting.
        This resource cannot be accessed anonymously.
      operationId: com.atlassian.jira.rest.v2.issue.GroupAndUserPickerResource.findUsersAndGroups_get
      x-api-path-slug: api2groupuserpicker-get
      parameters:
      - in: query
        name: avatarSize
        description: The size of the avatar to return
      - in: query
        name: caseInsensitive
        description: whether the search for groups should be case insensitive
      - in: query
        name: excludeConnectAddons
        description: Boolean indicating whether Connect Add-on users and groups should
          be excluded from the search results
      - in: query
        name: fieldId
        description: The custom field id, if this request comes from a custom field,
          such as a user picker
      - in: query
        name: issueTypeId
        description: The list of issue type ids to further restrict the search
      - in: query
        name: maxResults
        description: the maximum number of users to return (defaults to 50)
      - in: query
        name: projectId
        description: The list of project ids to further restrict the search This parameter
          can occur multiple times to pass in multiple project ids
      - in: query
        name: query
        description: A string used to search username, Name or e-mail address
      - in: query
        name: showAvatar
        description: If the user avatar should be returned or not
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Groups
  /api/2/user/groups:
    get:
      summary: Get user groups
      description: Returns the groups to which a user belongs. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
        _Browse users and groups_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.getUserGroups_get
      x-api-path-slug: api2usergroups-get
      parameters:
      - in: query
        name: accountId
        description: The account ID of the user
      - in: header
        name: force-account-id
      - in: query
        name: key
        description: The key of the user
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - User
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