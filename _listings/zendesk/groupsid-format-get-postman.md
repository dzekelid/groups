{
  "info": {
    "name": "Sales Force Desk API Get Group",
    "_postman_id": "c38b4fe6-e515-4a6e-ba34-7e58b09dbf26",
    "description": "Get group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "3df50030-60fc-486a-8980-bf89ab84e9cf",
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
              "id": "7c60573b-324e-4cbe-93c8-35a6f0452ee0"
            }
          ]
        },
        {
          "id": "164fab74-14b8-4afe-a89d-80a25e2db6dd",
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
              "id": "c94c8148-8519-481a-a11e-873b575ead7b"
            }
          ]
        }
      ]
    }
  ]
}