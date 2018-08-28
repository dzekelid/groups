{
  "info": {
    "name": "Azure API Management API Groups ListByService",
    "_postman_id": "f5e00e8b-f5c6-4b86-bb18-9cd32925183e",
    "description": "Lists a collection of groups defined within a service instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "07b1ecf3-d765-4e39-83dc-6c62645eee41",
          "name": "Groups_ListByService",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/groups"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a collection of groups defined within a service instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a20cc28-d4dd-4210-87a0-5193b5454679"
            }
          ]
        }
      ]
    }
  ]
}