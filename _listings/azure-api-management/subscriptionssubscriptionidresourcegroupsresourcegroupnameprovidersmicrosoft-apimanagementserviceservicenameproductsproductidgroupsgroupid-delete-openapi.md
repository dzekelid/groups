---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API ProductGroups Delete
  description: Deletes the association between the specified group and product.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups
  : get:
      summary: Groups ListByService
      description: Lists a collection of groups defined within a service instance.
      operationId: Groups_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroups-get
      parameters:
      - in: query
        name: $filter
        description: '| Field       | Supported operators    | Supported functions                         ||-------------|------------------------|---------------------------------------------||
          id          | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || name        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || description | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || type        | eq, ne                 |
          N/A                                         |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Groups
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/groups/{groupId}
  : get:
      summary: Groups Get
      description: Gets the details of the group specified by its identifier.
      operationId: Groups_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Groups CreateOrUpdate
      description: Creates or Updates a group.
      operationId: Groups_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
    patch:
      summary: Groups Update
      description: Updates the details of the group specified by its identifier.
      operationId: Groups_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupid-patch
      parameters:
      - in: header
        name: If-Match
        description: ETag of the Group Entity
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
    delete:
      summary: Groups Delete
      description: Deletes specific group of the API Management service instance.
      operationId: Groups_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamegroupsgroupid-delete
      parameters:
      - in: header
        name: If-Match
        description: ETag of the Group Entity
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Groups
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/products/{productId}/groups
  : get:
      summary: ProductGroups ListByProducts
      description: Lists the collection of developer groups associated with the specified
        product.
      operationId: ProductGroups_ListByProducts
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameproductsproductidgroups-get
      parameters:
      - in: query
        name: $filter
        description: '| Field       | Supported operators    | Supported functions                         ||-------------|------------------------|---------------------------------------------||
          id          | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || name        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || description | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || type        | eq, ne                 |
          N/A                                         |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Product Groups
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/products/{productId}/groups/{groupId}
  : put:
      summary: ProductGroups Create
      description: Adds the association between the specified developer group with
        the specified product.
      operationId: ProductGroups_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameproductsproductidgroupsgroupid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Product Groups
    delete:
      summary: ProductGroups Delete
      description: Deletes the association between the specified group and product.
      operationId: ProductGroups_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameproductsproductidgroupsgroupid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Product Groups
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