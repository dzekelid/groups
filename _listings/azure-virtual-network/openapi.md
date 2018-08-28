---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 1
info:
  title: NetworkManagementClient
  description: the-microsoft-azure-network-management-api-provides-a-restful-set-of-web-services-that-interact-with-microsoft-azure-networks-service-to-manage-your-network-resources--the-api-has-entities-that-capture-the-relationship-between-an-end-user-and-the-microsoft-azure-networks-service-
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
---