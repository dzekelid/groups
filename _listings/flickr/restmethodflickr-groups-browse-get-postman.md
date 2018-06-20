{
  "info": {
    "name": "Flickr Groups Browse",
    "_postman_id": "4342072b-52bc-442a-b77b-781b13cc69f8",
    "description": "Browse the group category tree, finding groups and sub-categories.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "e4e9b0f1-2a8c-44ee-9e7e-7b2f6afde88b",
          "name": "getRestMethodFlickr.groups.browse",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.browse?api_key=%7B%7D&cat_id=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Browse the group category tree, finding groups and sub-categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9afb4cab-d207-4a2c-b258-797ecb760fd3"
            }
          ]
        }
      ]
    }
  ]
}