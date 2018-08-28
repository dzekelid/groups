swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{page}/groups:
    get:
      summary: Get Page Groups
      description: The groups this page is a member of
      operationId: getPageGroups
      x-api-path-slug: pagegroups-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Groups
  /{user}/groups:
    get:
      summary: Get User Groups
      description: The Groups that the user belongs to.
      operationId: getUserGroups
      x-api-path-slug: usergroups-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
  /{group}:
    get:
      summary: Get Group
      description: A Facebook group
      operationId: getGroup
      x-api-path-slug: group-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
  /{group}/feed:
    get:
      summary: Get Group Feed
      description: This group's wall
      operationId: getGroupFeed
      x-api-path-slug: groupfeed-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
    post:
      summary: Post Group Feed
      description: Posts a status message on this group's wall
      operationId: postGroupFeed
      x-api-path-slug: groupfeed-post
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Group
      - Feed
  /{group}/members:
    get:
      summary: Get Group Members
      description: All of the users who are members of this group
      operationId: getGroupMembers
      x-api-path-slug: groupmembers-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Members
  /{group}/picture:
    get:
      summary: Get Group Picture
      description: The profile picture of this group
      operationId: getGroupPicture
      x-api-path-slug: grouppicture-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Group
      - Picture
  /{group}/docs:
    get:
      summary: Get Group Docs
      description: The docs in this group
      operationId: getGroupDocs
      x-api-path-slug: groupdocs-get
      parameters:
      - in: path
        name: group
        description: Represents the ID of the group object
      responses:
        200:
          description: OK
      tags:
      - Group
      - Docs