{
  "info": {
    "name": "Azure Virtual Network API Network Security Groups Delete",
    "_postman_id": "cf00f45c-d89a-4c80-bd94-df0b45c09f7b",
    "description": "Deletes the specified network security group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network security groups",
      "item": [
        {
          "id": "2c44e157-4499-43ea-992d-a91c945f45fd",
          "name": "NetworkSecurityGroups_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkSecurityGroups/:networkSecurityGroupName"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified network security group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "137f81e8-edf2-4fd6-bb6e-ab4f4c68b3ba"
            }
          ]
        }
      ]
    }
  ]
}