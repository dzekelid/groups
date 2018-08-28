{
  "info": {
    "name": "Google Cloud User Accounts API Get Groups",
    "_postman_id": "7e5db3cb-fc4b-47b4-83f1-53e6fa0d41de",
    "description": "Retrieves the list of groups contained within the specified project.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "c93eea41-9137-4117-9dac-32ca8971bb86",
          "name": "clouduseraccounts.groups.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "clouduseraccounts",
                "vm_alpha",
                "projects",
                ":project/global/groups"
              ],
              "query": [
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "project",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the list of groups contained within the specified project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da6b6ae7-2f93-4816-ab6b-31d0149c1e6d"
            }
          ]
        }
      ]
    }
  ]
}