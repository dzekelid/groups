{
  "info": {
    "name": "One Note Get Notebooks Notebookid Sectiongroups",
    "_postman_id": "f9a7803e-ffda-464e-94cf-376ca246d031",
    "description": "Returns a collection of section groups within a specific notebook.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notebooks",
      "item": [
        {
          "id": "39c7fa61-0cac-43f3-be8b-f8f4ad148734",
          "name": "getNotebooksNotebookSectiongroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "notebooks/:notebookId/sectiongroups"
              ],
              "query": [
                {
                  "key": "count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderby",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "select",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "top",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "notebookId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of section groups within a specific notebook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58f35918-b1d8-478b-9132-0315f8027e02"
            }
          ]
        }
      ]
    }
  ]
}