---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Network Security Groups List
  description: Gets all network security groups in a resource group.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkSecurityGroups/{networkSecurityGroupName}
  : delete:
      summary: Network Security Groups Delete
      description: Deletes the specified network security group.
      operationId: NetworkSecurityGroups_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworksecuritygroupsnetworksecuritygroupname-delete
      parameters:
      - in: path
        name: networkSecurityGroupName
        description: The name of the network security group
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Security Groups
    get:
      summary: Network Security Groups Get
      description: Gets the specified network security group.
      operationId: NetworkSecurityGroups_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworksecuritygroupsnetworksecuritygroupname-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced resources
      - in: path
        name: networkSecurityGroupName
        description: The name of the network security group
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Security Groups
    put:
      summary: Network Security Groups Create Or Update
      description: Creates or updates a network security group in the specified resource
        group.
      operationId: NetworkSecurityGroups_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworksecuritygroupsnetworksecuritygroupname-put
      parameters:
      - in: path
        name: networkSecurityGroupName
        description: The name of the network security group
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create or update network security
          group operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Security Groups
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/networkSecurityGroups:
    get:
      summary: Network Security Groups List All
      description: Gets all network security groups in a subscription.
      operationId: NetworkSecurityGroups_ListAll
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-networknetworksecuritygroups-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Network Security Groups
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkSecurityGroups:
    get:
      summary: Network Security Groups List
      description: Gets all network security groups in a resource group.
      operationId: NetworkSecurityGroups_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworksecuritygroups-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Security Groups
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