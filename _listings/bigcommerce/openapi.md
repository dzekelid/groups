swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/customers/subscribers:
    delete:
      summary: Delete a group of subscribers by parameter
      description: ""
      operationId: V3CustomersSubscribersByStoreHashDelete
      x-api-path-slug: store-hashv3customerssubscribers-delete
      parameters:
      - in: query
        name: date_created
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Group
      - Of
      - Subscribers
      - By
      - Parameter