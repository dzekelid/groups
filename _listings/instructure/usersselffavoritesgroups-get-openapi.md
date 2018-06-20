---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API List favorite groups
  description: List favorite groups.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
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