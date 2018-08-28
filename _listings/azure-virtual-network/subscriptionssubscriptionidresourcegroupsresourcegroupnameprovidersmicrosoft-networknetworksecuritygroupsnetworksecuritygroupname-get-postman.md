{
  "info": {
    "name": "Azure Virtual Network API Network Security Groups Get",
    "_postman_id": "35811dac-96e5-46a1-bf91-a453aaf2927c",
    "description": "Gets the specified network security group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network security groups",
      "item": [
        {
          "id": "eb657a53-55ba-4865-9841-3b5b9fbe42ed",
          "name": "NetworkSecurityGroups_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkSecurityGroups/:networkSecurityGroupName"
              ],
              "query": [
                {
                  "key": "$expand",
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
                  "id": "networkSecurityGroupName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets the specified network security group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3af3f2b-989e-4599-a6c2-041c3c365c55"
            }
          ]
        }
      ]
    }
  ]
}