{
  "info": {
    "name": "Azure Event Hubs API Consumer Groups Delete",
    "_postman_id": "a0001ca5-2fca-421d-9310-28d9af59c0fb",
    "description": "Deletes a consumer group from the specified Event Hub and resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "consumer groups",
      "item": [
        {
          "id": "97d1199c-94a0-4e2d-955b-1f9eb502d086",
          "name": "ConsumerGroups_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.EventHub/namespaces/:namespaceName/eventhubs/:eventHubName/consumergroups/:consumerGroupName"
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
                  "id": "namespaceName",
                  "value": "namespaceName",
                  "type": "string"
                },
                {
                  "id": "eventHubName",
                  "value": "eventHubName",
                  "type": "string"
                },
                {
                  "id": "consumerGroupName",
                  "value": "consumerGroupName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a consumer group from the specified Event Hub and resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7be65306-e5d0-4ae4-8b33-b10b35ec25cc"
            }
          ]
        }
      ]
    }
  ]
}