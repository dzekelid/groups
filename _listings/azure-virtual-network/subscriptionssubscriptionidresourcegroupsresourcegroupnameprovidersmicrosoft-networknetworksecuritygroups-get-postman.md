{
  "info": {
    "name": "Azure Virtual Network API Network Security Groups List",
    "_postman_id": "0e0a7ebc-aa87-4c1e-a0ae-f1b778337ca1",
    "description": "Gets all network security groups in a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network security groups",
      "item": [
        {
          "id": "049ef384-3879-457d-9e9f-477105782e6b",
          "name": "NetworkSecurityGroups_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkSecurityGroups"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all network security groups in a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8062616d-e2ad-4d7c-b22c-8963313e392b"
            }
          ]
        }
      ]
    }
  ]
}