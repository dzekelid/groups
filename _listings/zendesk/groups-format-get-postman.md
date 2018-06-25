{
  "info": {
    "name": "Sales Force Desk API Get Groups",
    "_postman_id": "a2b26b3f-3870-4d23-a240-f3a1587f8dc3",
    "description": "Get groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "32d58433-6103-494d-91f3-97cea6df1559",
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
              "id": "26dbc692-1100-4131-9a85-4966124f5073"
            }
          ]
        }
      ]
    }
  ]
}