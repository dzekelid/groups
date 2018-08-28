{
  "info": {
    "name": "Azure API Management API Groups Get",
    "_postman_id": "468b9cbb-baa4-44b0-9bf0-b1ff23d70de0",
    "description": "Gets the details of the group specified by its identifier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "5638f9d2-9406-4aeb-aeb5-0ce8fd9801e9",
          "name": "Groups_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/groups/:groupId"
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
                  "id": "groupId",
                  "value": "groupId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the details of the group specified by its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c262e6d9-7ef0-40f3-b341-d2bfdd79e3f7"
            }
          ]
        }
      ]
    }
  ]
}