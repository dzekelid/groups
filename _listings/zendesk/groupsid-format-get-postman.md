{
  "info": {
    "name": "Sales Force Desk API Get Group",
    "_postman_id": "925c6be0-27a3-47db-856a-c72cd4c80554",
    "description": "Get group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "bf4a89b1-2c9a-45c3-b624-6d47bcf7a682",
          "name": "get-groups",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/groups.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d92feb0-febd-4f9b-b71b-ea6f31a52245"
            }
          ]
        },
        {
          "id": "a84c35fb-6629-475e-b783-dccc7b57877e",
          "name": "get-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "yoursite.desk.com",
              "path": [
                "api",
                "v2",
                "groups/:id.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf9a9e27-229e-4541-82b9-295806b7ee0b"
            }
          ]
        }
      ]
    }
  ]
}