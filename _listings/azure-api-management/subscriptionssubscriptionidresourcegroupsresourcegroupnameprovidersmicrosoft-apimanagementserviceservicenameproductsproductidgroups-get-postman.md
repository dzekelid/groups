{
  "info": {
    "name": "Azure API Management API ProductGroups ListByProducts",
    "_postman_id": "9080f4ea-7737-4938-8ede-d383f1f15269",
    "description": "Lists the collection of developer groups associated with the specified product.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "product groups",
      "item": [
        {
          "id": "bd768100-7c3c-4afb-885f-5ed0edeacd79",
          "name": "ProductGroups_ListByProducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/products/:productId/groups"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the collection of developer groups associated with the specified product"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eadf0245-6558-4270-9807-3f2324050a5f"
            }
          ]
        }
      ]
    }
  ]
}