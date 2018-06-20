{
  "info": {
    "name": "Instructure Canvas Global API Import an outcome group",
    "_postman_id": "9b90ce5f-a91b-4e3c-879a-e40627ffa543",
    "description": "Import an outcome group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Global",
      "item": [
        {
          "id": "4c74e504-e4e6-4630-ae3c-8b2a0d1ec79d",
          "name": "show-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "global/outcome_groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "320addf2-3417-4977-935d-853196e65fca"
            }
          ]
        },
        {
          "id": "ca23f53f-ef58-47a4-a0f1-675a3ba5b55b",
          "name": "update-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "global/outcome_groups/:id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_outcome_group_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vendor_guid",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc08d104-b84e-455a-a169-7ee2954265e8"
            }
          ]
        },
        {
          "id": "55c28d1a-1cba-46b6-8e77-805d04760d50",
          "name": "delete-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "global/outcome_groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f096410-b142-4a5b-862c-a31f776f5957"
            }
          ]
        },
        {
          "id": "1820dd38-c233-41d4-86d6-548c04477821",
          "name": "import-an-outcome-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "global/outcome_groups/:id/import"
              ],
              "query": [
                {
                  "key": "source_outcome_group_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Import an outcome group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d1332eb-2653-4d50-b603-ecaea55e3fa8"
            }
          ]
        }
      ]
    }
  ]
}