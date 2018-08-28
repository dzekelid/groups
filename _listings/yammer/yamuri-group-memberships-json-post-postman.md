{
  "info": {
    "name": "Yammer API Create Join A Group",
    "_postman_id": "47e87bdd-4982-4bac-ad9e-34d04fbd9295",
    "description": "Join the group specified by the numeric string ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "78fbeb05-b7e5-4944-b957-599407782a5a",
          "name": "Create_Join a group_",
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
            "method": "POST",
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
              "id": "2eea494d-6435-4eaf-b87a-0478e8f04878"
            }
          ]
        }
      ]
    }
  ]
}