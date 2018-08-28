{
  "info": {
    "name": "Azure API Management API ProductGroups Delete",
    "_postman_id": "f7ae7672-af21-4069-bae9-27e0023af9c5",
    "description": "Deletes the association between the specified group and product.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "product groups",
      "item": [
        {
          "id": "72087aa9-0c26-4a62-bea8-135cc5eb7d1b",
          "name": "ProductGroups_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the association between the specified group and product"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "611104be-7adf-4736-bd11-a4e357287301"
            }
          ]
        }
      ]
    }
  ]
}