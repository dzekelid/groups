---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Delete Shipping Groups
  description: Delete shipping groups.
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