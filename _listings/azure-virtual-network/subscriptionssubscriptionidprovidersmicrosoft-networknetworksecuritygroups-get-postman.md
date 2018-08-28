{
  "info": {
    "name": "Azure Virtual Network API Network Security Groups List All",
    "_postman_id": "ebb8094b-85fb-48e1-b678-dfd47cc2cafc",
    "description": "Gets all network security groups in a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network security groups",
      "item": [
        {
          "id": "4addf1e4-56c5-4278-8418-03e5c947177c",
          "name": "NetworkSecurityGroups_ListAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/networkSecurityGroups"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all network security groups in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "280ad459-fd56-4bdb-b0cd-8ad63b8347d9"
            }
          ]
        }
      ]
    }
  ]
}