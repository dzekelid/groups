{
  "info": {
    "name": "Yammer API Delete Leave A Group",
    "_postman_id": "9836e056-d8b9-426f-aea4-5dd8039c0ace",
    "description": "Join the group specified by the numeric string ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "2cc9d6ed-c524-4ce6-8c6d-1f3db0d948b2",
          "name": "Delete_Leave a group_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/group_memberships.json"
              ],
              "query": [
                {
                  "key": "group_id",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Join the group specified by the numeric string ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0abeb1b-64aa-401e-b1a6-0e0041f2ef16"
            }
          ]
        }
      ]
    }
  ]
}