swagger: "2.0"
x-collection-name: Slack
x-complete: 1
info:
  title: Slack
  description: one-way-to-interact-with-the-slack-platform-is-its-http-rpcbased-web-api-a-collection-of-methods-requiring-oauth-2-0based-user-bot-or-workspace-tokens-blessed-with-related-oauth-scopes-
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups.replies:
    get:
      summary: Get Group Thread
      description: Retrieve a thread of messages posted to a private channel
      operationId: groups_replies
      x-api-path-slug: groups-replies-get
      parameters:
      - in: query
        name: channel
        description: Private channel to fetch thread from
      - in: query
        name: thread_ts
        description: Unique identifier of a threads parent message
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.rename:
    post:
      summary: Rename Group
      description: Renames a private channel.
      operationId: groups_rename
      x-api-path-slug: groups-rename-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to rename
      - in: formData
        name: name
        description: New name for private channel
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: validate
        description: Whether to return errors on invalid channel name instead of modifying
          it to meet the specified criteria
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.list:
    get:
      summary: Get Group
      description: Lists private channels that the calling user has access to.
      operationId: groups_list
      x-api-path-slug: groups-list-get
      parameters:
      - in: query
        name: exclude_archived
        description: Dont return archived private channels
      - in: query
        name: exclude_members
        description: Exclude the `members` from each `group`
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.kick:
    post:
      summary: Remove User From Group
      description: Removes a user from a private channel.
      operationId: groups_kick
      x-api-path-slug: groups-kick-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to remove user from
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: User to remove from private channel
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.mark:
    post:
      summary: Mark Group
      description: Sets the read cursor in a private channel.
      operationId: groups_mark
      x-api-path-slug: groups-mark-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to set reading cursor in
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: ts
        description: Timestamp of the most recently seen message
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.users.list:
    get:
      summary: List Group Users
      description: List all users in a User Group
      operationId: usergroups_users_list
      x-api-path-slug: usergroups-users-list-get
      parameters:
      - in: query
        name: include_disabled
        description: Allow results that involve disabled User Groups
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: usergroup
        description: The encoded ID of the User Group to update
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.info:
    get:
      summary: Get Group
      description: Gets information about a private channel.
      operationId: groups_info
      x-api-path-slug: groups-info-get
      parameters:
      - in: query
        name: channel
        description: Private channel to get info on
      - in: query
        name: include_locale
        description: Set this to `true` to receive the locale for this group
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.users.update:
    post:
      summary: Update Group Users
      description: Update the list of users for a User Group
      operationId: usergroups_users_update
      x-api-path-slug: usergroups-users-update-post
      parameters:
      - in: formData
        name: include_count
        description: Include the number of users in the User Group
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: usergroup
        description: The encoded ID of the User Group to update
      - in: formData
        name: users
        description: A comma separated string of encoded user IDs that represent the
          entire list of users for the User Group
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.update:
    post:
      summary: Update Group
      description: Update an existing User Group
      operationId: usergroups_update
      x-api-path-slug: usergroups-update-post
      parameters:
      - in: formData
        name: channels
        description: A comma separated string of encoded channel IDs for which the
          User Group uses as a default
      - in: formData
        name: description
        description: A short description of the User Group
      - in: formData
        name: handle
        description: A mention handle
      - in: formData
        name: include_count
        description: Include the number of users in the User Group
      - in: formData
        name: name
        description: A name for the User Group
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: usergroup
        description: The encoded ID of the User Group to update
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.leave:
    post:
      summary: Leave Group
      description: Leaves a private channel.
      operationId: groups_leave
      x-api-path-slug: groups-leave-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to leave
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.create:
    post:
      summary: Create Group
      description: Create a User Group
      operationId: usergroups_create
      x-api-path-slug: usergroups-create-post
      parameters:
      - in: formData
        name: channels
        description: A comma separated string of encoded channel IDs for which the
          User Group uses as a default
      - in: formData
        name: description
        description: A short description of the User Group
      - in: formData
        name: handle
        description: A mention handle
      - in: formData
        name: include_count
        description: Include the number of users in each User Group
      - in: formData
        name: name
        description: A name for the User Group
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.createChild:
    post:
      summary: Create Child Group
      description: Clones and archives a private channel.
      operationId: groups_createChild
      x-api-path-slug: groups-createchild-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to clone and archive
      - in: formData
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - archives
  /usergroups.enable:
    post:
      summary: Enable Group
      description: Enable a User Group
      operationId: usergroups_enable
      x-api-path-slug: usergroups-enable-post
      parameters:
      - in: formData
        name: include_count
        description: Include the number of users in the User Group
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: usergroup
        description: The encoded ID of the User Group to enable
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.invite:
    post:
      summary: Invite User To Group
      description: Invites a user to a private channel.
      operationId: groups_invite
      x-api-path-slug: groups-invite-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to invite user to
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: user
        description: User to invite
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.create:
    post:
      summary: Create Group
      description: Creates a private channel.
      operationId: groups_create
      x-api-path-slug: groups-create-post
      parameters:
      - in: formData
        name: name
        description: Name of private channel to create
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: validate
        description: Whether to return errors on invalid channel name instead of modifying
          it to meet the specified criteria
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.list:
    get:
      summary: List Groups
      description: List all User Groups for a team
      operationId: usergroups_list
      x-api-path-slug: usergroups-list-get
      parameters:
      - in: query
        name: include_count
        description: Include the number of users in each User Group
      - in: query
        name: include_disabled
        description: Include disabled User Groups
      - in: query
        name: include_users
        description: Include the list of users for each User Group
      - in: query
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.open:
    post:
      summary: Open Group
      description: Opens a private channel.
      operationId: groups_open
      x-api-path-slug: groups-open-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to open
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.history:
    get:
      summary: Group History
      description: Fetches history of messages and events from a private channel.
      operationId: groups_history
      x-api-path-slug: groups-history-get
      parameters:
      - in: query
        name: channel
        description: Private channel to fetch history for
      - in: query
        name: count
        description: Number of messages to return, between 1 and 1000
      - in: query
        name: inclusive
        description: Include messages with latest or oldest timestamp in results
      - in: query
        name: latest
        description: End of time range of messages to include in results
      - in: query
        name: oldest
        description: Start of time range of messages to include in results
      - in: query
        name: token
        description: Authentication token
      - in: query
        name: unreads
        description: Include `unread_count_display` in the output?
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.setTopic:
    post:
      summary: Set Group Topic
      description: Sets the topic for a private channel.
      operationId: groups_setTopic
      x-api-path-slug: groups-settopic-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to set the topic of
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: topic
        description: The new topic
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /usergroups.disable:
    post:
      summary: Disable Group
      description: Disable an existing User Group
      operationId: usergroups_disable
      x-api-path-slug: usergroups-disable-post
      parameters:
      - in: formData
        name: include_count
        description: Include the number of users in the User Group
      - in: header
        name: token
        description: Authentication token
      - in: formData
        name: usergroup
        description: The encoded ID of the User Group to disable
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.setPurpose:
    post:
      summary: Set Group Purpose
      description: Sets the purpose for a private channel.
      operationId: groups_setPurpose
      x-api-path-slug: groups-setpurpose-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to set the purpose of
      - in: formData
        name: purpose
        description: The new purpose
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
  /groups.unarchive:
    post:
      summary: Unarchive Group
      description: Unarchives a private channel.
      operationId: groups_unarchive
      x-api-path-slug: groups-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - Archives
  /groups.archive:
    post:
      summary: Archive Group
      description: Archives a private channel.
      operationId: groups_archive
      x-api-path-slug: groups-archive-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to archive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - Archives