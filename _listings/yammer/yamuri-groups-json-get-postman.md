{
  "info": {
    "name": "Yammer API List Active Groups",
    "_postman_id": "3689fe1f-c55f-4a76-abee-1e5ac4117513",
    "description": "List activity groups",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "f8e95bd9-4d0f-4706-9583-79708f055a9f",
          "name": "List Active Groups_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/groups.json"
              ],
              "query": [
                {
                  "key": "sort_by",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List activity groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0380c893-8ed6-4f0d-b191-93cd8fe2f895"
            }
          ]
        }
      ]
    }
  ]
}