{
  "info": {
    "name": "Flickr Groups Search",
    "_postman_id": "818c4c95-538a-44c9-a655-f4d43982f08f",
    "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "e7619575-a860-475c-beb3-3a3a73f0ba65",
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
              "id": "924480b5-9a8e-4c9b-8b8e-f4459d193c88"
            }
          ]
        },
        {
          "id": "187b60da-89e1-4fa3-a6dd-e431187c27fc",
          "name": "getRestMethodFlickr.groups.getinfo",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.getInfo?api_key=%7B%7D&format=%7B%7D&group_id=%7B%7D&lang=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d77a5a5a-9e91-439f-bf3e-425abc9263cd"
            }
          ]
        },
        {
          "id": "dcac1cb2-14f8-4abe-ae57-a72adb1f28b6",
          "name": "getRestMethodFlickr.groups.search",
          "request": {
            "url": "http://api.flickr.com/services/rest/?method=flickr.groups.search?api_key=%7B%7D&format=%7B%7D&page=%7B%7D&per_page=%7B%7D&text=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for groups. 18+ groups will only be returned for authenticated calls where the authenticated user is over 18."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12262ed7-7223-4c9c-9ad4-f9a154803877"
            }
          ]
        }
      ]
    }
  ]
}