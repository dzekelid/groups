{
  "info": {
    "name": "Azure Event Hubs API Consumer Groups Get",
    "_postman_id": "7dd65d92-c972-4ede-9d1e-a025a06a47a2",
    "description": "Gets a description for the specified consumer group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "consumer groups",
      "item": [
        {
          "id": "11ebd137-0d4f-4ccf-a1b3-1db005f283bf",
          "name": "ConsumerGroups_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a description for the specified consumer group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46785388-e60e-41c7-a6ce-1d7ab0c15d50"
            }
          ]
        }
      ]
    }
  ]
}