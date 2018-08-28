swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shipping/{cartId}/groups:
    get:
      summary: Get Shipping Groups
      description: Get shipping groups.
      operationId: getShippingCartGroups
      x-api-path-slug: shippingcartidgroups-get
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Groups
    delete:
      summary: Delete Shipping Groups
      description: Delete shipping groups.
      operationId: deleteShippingCartGroups
      x-api-path-slug: shippingcartidgroups-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Groups
  /shipping/{cartId}/group:
    post:
      summary: Post Shipping Group
      description: Post shipping group.
      operationId: postShippingCartGroup
      x-api-path-slug: shippingcartidgroup-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
  /shipping/{cartId}/group/{fulfillmentGroupId}:
    delete:
      summary: Delete Shipping Group Fulfillmentgroupid
      description: Delete shipping group fulfillmentgroupid.
      operationId: deleteShippingCartGroupFulfillmentgroup
      x-api-path-slug: shippingcartidgroupfulfillmentgroupid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
    patch:
      summary: Patch Shipping Group Fulfillmentgroupid
      description: Patch shipping group fulfillmentgroupid.
      operationId: patchShippingCartGroupFulfillmentgroup
      x-api-path-slug: shippingcartidgroupfulfillmentgroupid-patch
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
  /shipping/{cartId}/group/{fulfillmentGroupId}/item:
    post:
      summary: Post Shipping Group Fulfillmentgroupid Item
      description: Post shipping group fulfillmentgroupid item.
      operationId: postShippingCartGroupFulfillmentgroupItem
      x-api-path-slug: shippingcartidgroupfulfillmentgroupiditem-post
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: wrapper
        description: wrapper
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Item
  /shipping/{cartId}/group/{fulfillmentGroupId}/item/{itemId}:
    delete:
      summary: Delete Shipping Group Fulfillmentgroupid Item
      description: Delete shipping group fulfillmentgroupid item.
      operationId: deleteShippingCartGroupFulfillmentgroupItemItem
      x-api-path-slug: shippingcartidgroupfulfillmentgroupiditemitemid-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: path
        name: itemId
        description: itemId
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Item
  /shipping/{cartId}/group/{fulfillmentGroupId}/option/{fulfillmentOptionId}:
    put:
      summary: Put Shipping Group Fulfillmentgroupid Option Fulfillmentoptionid
      description: Put shipping group fulfillmentgroupid option fulfillmentoptionid.
      operationId: putShippingCartGroupFulfillmentgroupOptionFulfillmentoption
      x-api-path-slug: shippingcartidgroupfulfillmentgroupidoptionfulfillmentoptionid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: path
        name: fulfillmentOptionId
        description: fulfillmentOptionId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Option
      - Fulfillmentoptionid