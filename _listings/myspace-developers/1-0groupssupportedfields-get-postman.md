{
  "info": {
    "name": "My Space Get Groups Supported Fields",
    "_postman_id": "c13be715-8fbd-4f50-9e1a-b9f9e88d4df2",
    "description": "Retrieves all supported fields.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "326ec29f-8469-4217-b0fc-26237b9c9b47",
          "name": "1.0.groups.personId.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.myspace.com",
              "path": [
                "1.0/groups/:personId"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "msPrivacyLevel",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startIndex",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "personId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current user's groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3df8952a-ec83-47e1-bc98-e2a3de2d2924"
            }
          ]
        },
        {
          "id": "b2d4c099-9a64-4d12-b858-c3f0088cec27",
          "name": "1.0.groups._supportedFields.get",
          "request": {
            "url": "http://api.myspace.com/1.0/groups/@supportedFields?count=%7B%7D&fields=%7B%7D&format=%7B%7D&msPrivacyLevel=%7B%7D&startIndex=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves all supported fields."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ca33d35-6c87-4a75-b98e-bf6b00dfb737"
            }
          ]
        }
      ]
    }
  ]
}