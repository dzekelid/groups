{
  "info": {
    "name": "Azure API Management API Groups Delete",
    "_postman_id": "b80d3ffd-d17a-43c6-a790-b3c966ea812b",
    "description": "Deletes specific group of the API Management service instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "80b7e49e-432f-4381-a0c2-321406e83098",
          "name": "Groups_Delete",
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
            "method": "DELETE",
            "header": [
              {
                "key": "If-Match",
                "value": "{}",
                "description": "ETag of the Group Entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes specific group of the API Management service instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8d38174-59b7-45ec-89be-eba4d6410077"
            }
          ]
        }
      ]
    }
  ]
}