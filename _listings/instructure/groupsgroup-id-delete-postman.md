{
  "info": {
    "name": "Instructure Canvas Groups API Delete a group",
    "_postman_id": "04673264-8deb-455b-ab68-756c02f028a1",
    "description": "Delete a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "b852914f-f27c-42aa-bfe5-9ce0e07e13a8",
          "name": "create-a-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/groups?description=%7B%7D&is_public=%7B%7D&join_level=%7B%7D&name=%7B%7D&storage_quota_mb=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44f797ec-b1bd-4133-9a16-7151f7052ba8"
            }
          ]
        },
        {
          "id": "39ff5cce-1ac6-4464-8903-d80ce1a99ccf",
          "name": "delete-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1de045c1-b0bf-4e37-be6c-dc72644ca636"
            }
          ]
        }
      ]
    }
  ]
}