---
swagger: "2.0"
x-collection-name: DNS Check
x-complete: 0
info:
  title: DNS Record Group Monitoring API Check Group
  description: The DNS Check API is used to request data for either a specific record
    group, or all DNS record groups owned by your account.
  version: v1
host: www.dnscheck.co
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/:group_uuid:
    get:
      summary: Check Group
      description: The DNS Check API is used to request data for either a specific
        record group, or all DNS record groups owned by your account.
      operationId: getGroups
      x-api-path-slug: groupsgroup-uuid-get
      parameters:
      - in: query
        name: api_key
        description: The secret key thats used to authenticate the connecting application
        type: string
        format: string
      - in: query
        name: group_uuid
        description: The UUID of the DNS record group
        type: string
        format: string
      responses:
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