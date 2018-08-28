---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Get groups
  x-api-slug: group-get
  description: |-
    Returns all user groups. The returned groups are ordered alphabetically in
    ascending order by group name.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/group-get-openapi.md
- name: The Confluence Cloud REST API - Add group to content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-put
  description: "Adds a group to a content restriction. That is, grant read or update
    \npermission to the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-openapi.md
- name: The Confluence Cloud REST API - Remove group from content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-delete
  description: "Removes a group from a content restriction. That is, remove read or
    update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-openapi.md
- name: The Confluence Cloud REST API - Get group
  x-api-slug: groupgroupname-get
  description: |-
    Returns a user group for a given group name.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupname-get-openapi.md
- name: The Confluence Cloud REST API - Get group members
  x-api-slug: groupgroupnamemember-get
  description: |-
    Returns the users that are members of a group.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupnamemember-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupnamemember-get-openapi.md
- name: The Confluence Cloud REST API - Get group memberships for user
  x-api-slug: usermemberof-get
  description: "Returns the groups that a user is a member of.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-openapi.md
- name: The Confluence Cloud REST API - Get group memberships for user
  x-api-slug: usermemberof-get
  description: "Returns the groups that a user is a member of.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-openapi.md
- name: The Confluence Cloud REST API - Get group memberships for user
  x-api-slug: usermemberof-get
  description: "Returns the groups that a user is a member of.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/usermemberof-get-openapi.md
- name: The Confluence Cloud REST API - Get group members
  x-api-slug: groupgroupnamemember-get
  description: |-
    Returns the users that are members of a group.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupnamemember-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupnamemember-get-openapi.md
- name: The Confluence Cloud REST API - Get group
  x-api-slug: groupgroupname-get
  description: |-
    Returns a user group for a given group name.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/groupgroupname-get-openapi.md
- name: The Confluence Cloud REST API - Remove group from content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-delete
  description: "Removes a group from a content restriction. That is, remove read or
    update \npermission for the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-delete-openapi.md
- name: The Confluence Cloud REST API - Add group to content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-put
  description: "Adds a group to a content restriction. That is, grant read or update
    \npermission to the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-openapi.md
- name: The Confluence Cloud REST API - Add group to content restriction
  x-api-slug: contentidrestrictionbyoperationoperationkeygroupgroupname-put
  description: "Adds a group to a content restriction. That is, grant read or update
    \npermission to the group for a piece of content.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to edit the content."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/contentidrestrictionbyoperationoperationkeygroupgroupname-put-openapi.md
- name: Jira Cloud REST API - Find groups
  x-api-slug: api2groupspicker-get
  description: |-
    Returns groups with substrings matching a given query. This is mainly for use with the group picker, so the returned groups contain html to be used as picker suggestions. The groups are also wrapped in a single response object that also contains a header for use in the picker, specifically _Showing X of Y matching groups_.

    The number of groups returned is limited by the system property "jira.ajax.autocomplete.limit"

    The groups will be unique and sorted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupspicker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupspicker-get-openapi.md
- name: Jira Cloud REST API - Find users and groups
  x-api-slug: api2groupuserpicker-get
  description: Returns a list of users and groups matching query with highlighting.
    This resource cannot be accessed anonymously.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuserpicker-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuserpicker-get-openapi.md
- name: Jira Cloud REST API - Get user groups
  x-api-slug: api2usergroups-get
  description: Returns the groups to which a user belongs. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Browse users and groups_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2usergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2usergroups-get-openapi.md
- name: Jira Cloud REST API - Get group
  x-api-slug: api2group-get
  description: |-
    This resource is deprecated, use [`group/member`](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-group-member-get).

    Returns all users in a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-openapi.md
- name: Jira Cloud REST API - Create group
  x-api-slug: api2group-post
  description: |-
    Creates a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-openapi.md
- name: Jira Cloud REST API - Remove group
  x-api-slug: api2group-delete
  description: |-
    Deletes a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-openapi.md
- name: Jira Cloud REST API - Get users from group
  x-api-slug: api2groupmember-get
  description: |-
    Returns all users in a group. Users are ordered by username.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-openapi.md
- name: Jira Cloud REST API - Add user to group
  x-api-slug: api2groupuser-post
  description: |-
    Adds a user to a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-openapi.md
- name: Jira Cloud REST API - Remove user from group
  x-api-slug: api2groupuser-delete
  description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-openapi.md
- name: Jira Cloud REST API - Get notification schemes paginated
  x-api-slug: api2notificationscheme-get
  description: |-
    Returns a [paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#pagination) list of [notification schemes](https://confluence.atlassian.com/x/8YdKLg) in order by display name.

    ### About notification schemes

    A notification scheme is a list of events and recipients who will receive notifications for those events. The list is contained within the `notificationSchemeEvents` object and contains pairs of `events` and `notifications`:

    *   `event` Identifies the type of event. The events can be [Jira system events](https://confluence.atlassian.com/x/8YdKLg#Creatinganotificationscheme-eventsEvents) or [custom events](https://confluence.atlassian.com/x/AIlKLg).
    *   `notifications` Identifies the [recipients](https://confluence.atlassian.com/x/8YdKLg#Creatinganotificationscheme-recipientsRecipients) of notifications for each event. Recipients can be any of the following types:

    *   `CurrentAssignee`
    *   `Reporter`
    *   `CurrentUser`
    *   `ProjectLead`
    *   `ComponentLead`
    *   `User` (the `parameter` is the user key)
    *   `Group` (the `parameter` is the group name)
    *   `ProjectRole` (the `parameter` is the project role ID)
    *   `EmailAddress`
    *   `AllWatchers`
    *   `UserCustomField` (the `parameter` is the ID of the custom field)
    *   `GroupCustomField`(the `parameter` is the ID of the custom field)

    _Note that you should allow for events without recipients to appear in responses._

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however the requesting user must have permission to administer at least one project associated with a notification scheme for it to be returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2notificationscheme-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2notificationscheme-get-openapi.md
- name: Jira Cloud REST API - Remove user from group
  x-api-slug: api2groupuser-delete
  description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-openapi.md
- name: Jira Cloud REST API - Remove user from group
  x-api-slug: api2groupuser-delete
  description: Removes a user from a group. **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):**
    _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-delete-openapi.md
- name: Jira Cloud REST API - Add user to group
  x-api-slug: api2groupuser-post
  description: |-
    Adds a user to a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-openapi.md
- name: Jira Cloud REST API - Add user to group
  x-api-slug: api2groupuser-post
  description: |-
    Adds a user to a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupuser-post-openapi.md
- name: Jira Cloud REST API - Get users from group
  x-api-slug: api2groupmember-get
  description: |-
    Returns all users in a group. Users are ordered by username.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-openapi.md
- name: Jira Cloud REST API - Get users from group
  x-api-slug: api2groupmember-get
  description: |-
    Returns all users in a group. Users are ordered by username.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2groupmember-get-openapi.md
- name: Jira Cloud REST API - Remove group
  x-api-slug: api2group-delete
  description: |-
    Deletes a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-openapi.md
- name: Jira Cloud REST API - Remove group
  x-api-slug: api2group-delete
  description: |-
    Deletes a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-delete-openapi.md
- name: Jira Cloud REST API - Create group
  x-api-slug: api2group-post
  description: |-
    Creates a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-openapi.md
- name: Jira Cloud REST API - Create group
  x-api-slug: api2group-post
  description: |-
    Creates a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-post-openapi.md
- name: Jira Cloud REST API - Get group
  x-api-slug: api2group-get
  description: |-
    This resource is deprecated, use [`group/member`](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-group-member-get).

    Returns all users in a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-openapi.md
- name: Jira Cloud REST API - Get group
  x-api-slug: api2group-get
  description: |-
    This resource is deprecated, use [`group/member`](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-group-member-get).

    Returns all users in a group.

    **[Permissions required](https://confluence.atlassian.com/x/FQiiLQ):** _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/atlassian/api2group-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---