---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 0
info:
  title: IBM Containers List all container groups in a space
  description: 'This endpoint returns a list of all container groups in a space independent
    of their current state. (corresponding IBM Containers command: `cf ic group list`).'
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/groups:
    get:
      summary: List all container groups in a space
      description: 'This endpoint returns a list of all container groups in a space
        independent of their current state. (corresponding IBM Containers command:
        `cf ic group list`).'
      operationId: this-endpoint-returns-a-list-of-all-container-groups-in-a-space-independent-of-their-current-state--
      x-api-path-slug: containersgroups-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
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