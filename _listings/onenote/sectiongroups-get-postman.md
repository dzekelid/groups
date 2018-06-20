{
  "info": {
    "name": "One Note Get Sectiongroups",
    "_postman_id": "66ff92e3-36d8-4ffc-b635-266a507b4557",
    "description": "Returns a collection of section groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SectionGroups",
      "item": [
        {
          "id": "7a1e952d-a599-4ae2-a140-e0f5b57d63be",
          "name": "getSectiongroups",
          "request": {
            "url": "http://www.onenote.com/api/v1.0/me/notes/sectionGroups/?count=%7B%7D&expand=%7B%7D&filter=%7B%7D&orderby=%7B%7D&select=%7B%7D&skip=%7B%7D&top=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of section groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db1576d9-e05c-417d-98ca-92292d6c6512"
            }
          ]
        }
      ]
    }
  ]
}