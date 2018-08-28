{
  "info": {
    "name": "Yammer API Get Suggested Groups And Users",
    "_postman_id": "07e735b8-6943-444f-aa3d-3c3dbdf23667",
    "description": "Show suggested groups to join and users to follow.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "groups",
      "item": [
        {
          "id": "4b8e764e-ba5a-4928-a9c9-aa1ab687781f",
          "name": "Get_Suggested Groups and Users_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                ":yamURI/suggestions.json"
              ],
              "variable": [
                {
                  "id": "yamURI",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show suggested groups to join and users to follow"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "377400c9-7cab-499d-a36a-df9c2a03cfd9"
            }
          ]
        }
      ]
    }
  ]
}