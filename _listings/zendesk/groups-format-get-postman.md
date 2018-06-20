{
  "info": {
    "name": "Sales Force Desk API Get Groups",
    "_postman_id": "f8a76dc3-9fb7-4b42-976b-6c2d42b36a19",
    "description": "Get groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "b69bf9bc-c672-41e8-a5a0-aa668ffa59a0",
          "name": "get-groups",
          "request": {
            "url": "http://yoursite.desk.com/api/v2/groups.json?format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "010991e0-00e4-418a-9fe2-23bdbb219892"
            }
          ]
        }
      ]
    }
  ]
}