{
  "info": {
    "name": "One Note Get Sectiongroups Sectiongroupid Sectiongroups",
    "_postman_id": "c867b37f-f7a5-45cb-91c4-80a3b2231433",
    "description": "Returns a collection of section groups within a specific section group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SectionGroups",
      "item": [
        {
          "id": "2a86d592-f681-4a51-8759-90ef846dc1fe",
          "name": "getSectiongroupsSectiongroupSectiongroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "sectionGroups/:sectionGroupId/sectionGroups"
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
            "description": "Returns a collection of section groups within a specific section group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0174857f-ccf0-42aa-92c8-ea52431aa3e6"
            }
          ]
        }
      ]
    }
  ]
}