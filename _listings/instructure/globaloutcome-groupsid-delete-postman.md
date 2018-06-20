{
  "info": {
    "name": "Instructure Canvas Global API Delete an outcome group",
    "_postman_id": "cd3d2035-3017-4597-8b51-5775691f39a7",
    "description": "Delete an outcome group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Global",
      "item": [
        {
          "id": "f2d87d1d-c38e-4a69-a901-5681c7cb5cbe",
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
              "id": "0937a755-8e4b-4120-ab9e-b51f770464e1"
            }
          ]
        }
      ]
    }
  ]
}