---
swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 0
info:
  title: Azure DocumentDB API Database Accounts List By Resource Group
  description: Lists all the Azure DocumentDB database accounts available under the
    given resource group.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts:
    get:
      summary: Database Accounts List By Resource Group
      description: Lists all the Azure DocumentDB database accounts available under
        the given resource group.
      operationId: DatabaseAccounts_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-documentdbdatabaseaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Database
      - Accounts
      - ListResource
      - Group
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