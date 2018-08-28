---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Group Add Favorite
  description: 'group: addFavorite Add the group to the list of the current user''s
    favorite groups. Supported for only Office 365 groups.'
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
  /directoryObjects/{id}/getMemberGroups:
    post:
      summary: Get Member Groups
      description: Get member groups Return all the groups that the specified user,
        group, or directory object is a member of. This function is transitive.
      operationId: GetMemberGroups
      x-api-path-slug: directoryobjectsidgetmembergroups-post
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
      - Member
      - Groups
  /groups:
    get:
      summary: List Groups
      description: List groups List all the groups available in an organization, including
        but not limited to Office 365 Groups. The default properties of each group
        are returned.
      operationId: ListGroups
      x-api-path-slug: groups-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
    post:
      summary: Create Group
      description: 'Create group Use this API to create a new group as specified in
        the request body. You can create one of 3 types of groups:'
      operationId: CreateGroup
      x-api-path-slug: groups-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
  /users/{id | userPrincipalName}/calendarGroups:
    get:
      summary: List Calendar Groups
      description: List calendarGroups Get the user's calendar groups.
      operationId: ListCalendarGroups
      x-api-path-slug: usersid--userprincipalnamecalendargroups-get
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
      - List
      - Calendar
      - Groups
    post:
      summary: Create Calendar Group
      description: Create CalendarGroup Use this API to create a new CalendarGroup.
      operationId: CreateCalendarGroup
      x-api-path-slug: usersid--userprincipalnamecalendargroups-post
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
      - Calendar
      - Group
  /me/calendarGroups/{id}:
    delete:
      summary: Delete Calendar Group
      description: Delete calendarGroup Delete a calendar group other than the default
        calendar group.
      operationId: DeleteCalendarGroup
      x-api-path-slug: mecalendargroupsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Group
    get:
      summary: Get Calendar Group
      description: Get calendarGroup Retrieve the properties and relationships of
        a calendar group object.
      operationId: GetCalendarGroup
      x-api-path-slug: mecalendargroupsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Group
  /users/{id | userPrincipalName}/calendarGroups/{id}:
    delete:
      summary: Delete Calendar Group
      description: Delete calendarGroup Delete a calendar group other than the default
        calendar group.
      operationId: DeleteCalendarGroup
      x-api-path-slug: usersid--userprincipalnamecalendargroupsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Group
    get:
      summary: Get Calendar Group
      description: Get calendarGroup Retrieve the properties and relationships of
        a calendar group object.
      operationId: GetCalendarGroup
      x-api-path-slug: usersid--userprincipalnamecalendargroupsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Group
  /groups/{id}/addFavorite:
    post:
      summary: Group Add Favorite
      description: 'group: addFavorite Add the group to the list of the current user''s
        favorite groups. Supported for only Office 365 groups.'
      operationId: Group:AddFavorite
      x-api-path-slug: groupsidaddfavorite-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - ""
      - Favorite
  /groups/{id}:
    delete:
      summary: Delete Group
      description: Delete group Delete group.
      operationId: DeleteGroup
      x-api-path-slug: groupsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
    get:
      summary: Get Group
      description: Get group Get the properties and relationships of a group object.
      operationId: GetGroup
      x-api-path-slug: groupsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
    patch:
      summary: Update Group
      description: Update group Update the properties of a group object.
      operationId: UpdateGroup
      x-api-path-slug: groupsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
  /groups/{id}/getMemberObjects:
    post:
      summary: Group Get Member Objects
      description: 'group: getMemberObjects Return all of the groups that this group
        is a member of. The check is transitive. Note: Groups cannot be members of
        directory roles, so no directory roles will be returned.'
      operationId: Group:GetMemberObjects
      x-api-path-slug: groupsidgetmemberobjects-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
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
      - Objects
  /groups/{id}/owners/$ref:
    post:
      summary: Add Group Owner
      description: Add group owner Add a user to the group's owners. The owners are
        a set of non-admin users who are allowed to modify the group object.
      operationId: AddGroupOwner
      x-api-path-slug: groupsidownersref-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Owner
  /groups/{id}/removeFavorite:
    post:
      summary: Group Remove Favorite
      description: 'group: removeFavorite Remove the group from the list of the current
        user''s favorite groups. Supported for only Office 365 groups.'
      operationId: Group:RemoveFavorite
      x-api-path-slug: groupsidremovefavorite-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Remove
      - Favorite
  /groups/{id}/resetUnseenCount:
    post:
      summary: Group Reset Unseen Count
      description: 'group: resetUnseenCount Reset the unseenCount of all the posts
        that the current user has not seen since their last visit. Supported for only
        Office 365 groups.'
      operationId: Group:ResetUnseenCount
      x-api-path-slug: groupsidresetunseencount-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Reset
      - Unseen
      - Count
  /groups/{id}/subscribeByMail:
    post:
      summary: Group Subscribe By Mail
      description: 'group: subscribeByMail Calling this method will enable the current
        user to receive email notifications for this group, about new posts, events,
        and files in that group. Supported for only Office 365 groups.'
      operationId: Group:SubscribeByMail
      x-api-path-slug: groupsidsubscribebymail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - SubscribeMail
  /groups/{id}/unsubscribeByMail:
    post:
      summary: Group Unsubscribe By Mail
      description: 'group: unsubscribeByMail Calling this method will prevent the
        current user from receiving email notifications for this group about new posts,
        events, and files in that group. Supported for only Office 365 groups.'
      operationId: Group:UnsubscribeByMail
      x-api-path-slug: groupsidunsubscribebymail-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - UnsubscribeMail
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