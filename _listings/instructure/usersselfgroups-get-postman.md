{
  "info": {
    "name": "Instructure Canvas Users API List your groups",
    "_postman_id": "6f8cdaa2-f9d2-4de2-903b-5f41c387a251",
    "description": "List your groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "8b6d1417-4099-4612-a965-bc47639a57bb",
          "name": "list-favorite-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "399e12ee-3622-45c1-911a-a8252f91f320"
            }
          ]
        },
        {
          "id": "bd8e4692-da97-498e-adaa-e41d49f6ac1b",
          "name": "reset-group-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset group favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2160e3ea-9389-401f-a5c7-fa4fc8f6517f"
            }
          ]
        },
        {
          "id": "a5c8317f-a381-4b91-bdac-84749fe7fd8a",
          "name": "add-group-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add group to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "280d7766-be3b-4c3c-8832-35cc9b5ed67a"
            }
          ]
        },
        {
          "id": "d3937ff8-4abd-4301-801b-b61b916a49ba",
          "name": "remove-group-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove group from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "450b493c-200a-4b53-822d-6607b6d3b251"
            }
          ]
        },
        {
          "id": "b22dcbc2-b6d4-425d-b236-57a0906da778",
          "name": "list-your-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/groups?context_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "244b4f3d-7c8b-4e67-9101-f473d70bc0bd"
            }
          ]
        }
      ]
    }
  ]
}