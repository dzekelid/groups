---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests multisignature groups data
  description: Searches for the specified account in the system and responds with
    a list of the multisignature groups that this account is member of.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{address}/multisignature_groups:
    get:
      summary: Requests multisignature groups data
      description: Searches for the specified account in the system and responds with
        a list of the multisignature groups that this account is member of.
      operationId: getMultisignatureGroups
      x-api-path-slug: accountsaddressmultisignature-groups-get
      parameters:
      - in: path
        name: address
        description: Lisk address of an account
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Multisignature
      - Groups
      - Data
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