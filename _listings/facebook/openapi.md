---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---