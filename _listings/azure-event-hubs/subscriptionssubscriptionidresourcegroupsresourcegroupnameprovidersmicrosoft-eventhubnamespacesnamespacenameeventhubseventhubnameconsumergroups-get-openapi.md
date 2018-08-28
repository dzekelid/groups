---
swagger: "2.0"
x-collection-name: Azure Event Hubs
x-complete: 0
info:
  title: Azure Event Hubs API Consumer Groups List All
  description: Gets all the consumer groups in a Namespace. An empty feed is returned
    if no consumer group exists in the Namespace.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/consumergroups/{consumerGroupName}
  : put:
      summary: Consumer Groups Create Or Update
      description: Creates or updates an Event Hubs consumer group as a nested resource
        within a Namespace.
      operationId: ConsumerGroups_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameconsumergroupsconsumergroupname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to create or update a consumer group resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Consumer Groups
    delete:
      summary: Consumer Groups Delete
      description: Deletes a consumer group from the specified Event Hub and resource
        group.
      operationId: ConsumerGroups_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameconsumergroupsconsumergroupname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Consumer Groups
    get:
      summary: Consumer Groups Get
      description: Gets a description for the specified consumer group.
      operationId: ConsumerGroups_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameconsumergroupsconsumergroupname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Consumer Groups
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventHub/namespaces/{namespaceName}/eventhubs/{eventHubName}/consumergroups
  : get:
      summary: Consumer Groups List All
      description: Gets all the consumer groups in a Namespace. An empty feed is returned
        if no consumer group exists in the Namespace.
      operationId: ConsumerGroups_ListAll
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-eventhubnamespacesnamespacenameeventhubseventhubnameconsumergroups-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Consumer Groups All
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