---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Me Groups
  description: Returns a collection of groups joined by logged-in user
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/groups.json:
    get:
      summary: Get Users Groups
      description: Returns a collection of groups joined by user with user id
      operationId: getUsersUserGroups.json
      x-api-path-slug: usersuser-idgroups-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Groups
  /me/groups.json:
    get:
      summary: Get Me Groups
      description: Returns a collection of groups joined by logged-in user
      operationId: getMeGroups.json
      x-api-path-slug: megroups-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Groups
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---