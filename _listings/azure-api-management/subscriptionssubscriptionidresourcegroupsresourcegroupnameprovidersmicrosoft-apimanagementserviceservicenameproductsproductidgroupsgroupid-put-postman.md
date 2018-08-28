{
  "info": {
    "name": "Azure API Management API ProductGroups Create",
    "_postman_id": "cb22be7c-c999-48e5-85e2-c91bc3a72a31",
    "description": "Adds the association between the specified developer group with the specified product.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "product groups",
      "item": [
        {
          "id": "db022c87-9c4c-4cfa-8458-576e60b858be",
          "name": "ProductGroups_Create",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/products/:productId/groups/:groupId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "productId",
                  "value": "productId",
                  "type": "string"
                },
                {
                  "id": "groupId",
                  "value": "groupId",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the association between the specified developer group with the specified product"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62dd8cc1-d16a-4d31-8ebc-2e2f8a7db1ef"
            }
          ]
        }
      ]
    }
  ]
}