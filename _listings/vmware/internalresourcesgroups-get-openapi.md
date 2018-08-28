---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get Custom Groups
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /internal/resources/groups:
    get:
      summary: Get Custom Groups
      description: 'TODO: Add Description'
      operationId: InternalResourcesGroupsGet
      x-api-path-slug: internalresourcesgroups-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: X-vRealizeOps-API-use-unsupported
      responses:
        200:
          description: OK
      tags:
      - Internal
      - Resources
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