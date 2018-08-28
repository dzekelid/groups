swagger: "2.0"
x-collection-name: Azure DocumentDB
x-complete: 1
info:
  title: DocumentDB
  description: azure-documentdb-database-service-resource-provider-rest-api
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