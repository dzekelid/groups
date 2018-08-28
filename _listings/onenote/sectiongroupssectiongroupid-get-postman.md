{
  "info": {
    "name": "One Note Get Sectiongroups Sectiongroupid",
    "_postman_id": "da80de17-6cc1-48fb-b925-2db3a2534f66",
    "description": "Returns a specific section group object.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SectionGroups",
      "item": [
        {
          "id": "cd5d6f67-0051-41e6-9925-826e11a6bf2a",
          "name": "getSectiongroupsSectiongroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "sectionGroups/:sectionGroupId"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "select",
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
            "description": "Returns a specific section group object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d32d1ed9-0e58-42d4-92c2-c67260bfb251"
            }
          ]
        }
      ]
    }
  ]
}