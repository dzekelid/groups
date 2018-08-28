{
  "info": {
    "name": "One Note Get Sectiongroups Sectiongroupid Sections",
    "_postman_id": "a6a61c45-1bee-4999-b8ec-b960feaccb7d",
    "description": "Returns a collection of sections within a specific section group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SectionGroups",
      "item": [
        {
          "id": "2be31f1e-0b3e-45be-9ae1-565f392b08a6",
          "name": "getSectiongroupsSectiongroupSections",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "sectionGroups/:sectionGroupId/sections"
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
                  "id": "sectionGroupId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of sections within a specific section group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b978dc2-9ac2-4be7-ba53-f9b07c6113ed"
            }
          ]
        }
      ]
    }
  ]
}