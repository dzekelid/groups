---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get groups
  description: |-
    Returns all user groups. The returned groups are ordered alphabetically in
    ascending order by group name.

    **[Permissions](https://confluence.atlassian.com/x/_AozKw) required**:
    Permission to access the Confluence site ('Can use' global permission).
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