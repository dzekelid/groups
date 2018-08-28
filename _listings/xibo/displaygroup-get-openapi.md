---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Get Display Groups
  description: ""
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /displaygroup:
    get:
      summary: Get Display Groups
      description: ""
      operationId: displayGroupSearch
      x-api-path-slug: displaygroup-get
      parameters:
      - in: formData
        name: displayGroup
        description: Filter by DisplayGroup Name
      - in: formData
        name: displayGroupId
        description: Filter by DisplayGroup Id
      - in: formData
        name: displayId
        description: Filter by DisplayGroups containing a specific display
      - in: formData
        name: dynamicCriteria
        description: Filter by DisplayGroups containing a specific dynamic criteria
      - in: formData
        name: forSchedule
        description: Should the list be refined for only those groups the User can
          Schedule against?
      - in: formData
        name: isDisplaySpecific
        description: Filter by whether the Display Group belongs to a Display or is
          user created
      - in: formData
        name: nestedDisplayId
        description: Filter by DisplayGroups containing a specific display in there
          nesting
      responses:
        200:
          description: OK
      tags:
      - Display
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