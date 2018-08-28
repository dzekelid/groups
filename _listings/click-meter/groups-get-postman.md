{
  "info": {
    "name": "Click Meter List of all the groups associated to the user.",
    "_postman_id": "a65f19bf-32d9-491a-8047-8d1188d6ed69",
    "description": "List of all the groups associated to the user..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Aggregated",
      "item": [
        {
          "id": "f7803105-37f9-4565-be51-03aa655ec742",
          "name": "getAggregatedSummaryGroups",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/aggregated/summary/groups?favourite=%7B%7D&fromDay=%7B%7D&limit=%7B%7D&offset=%7B%7D&sortBy=%7B%7D&sortDirection=%7B%7D&status=%7B%7D&tag=%7B%7D&textSearch=%7B%7D&timeFrame=%7B%7D&toDay=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve statistics about a subset of groups for a timeframe with groups data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "075604be-3b03-4ace-a21c-9e24fc4db7a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "ed38c2ca-586b-4a4d-8a87-3ff1680d9f27",
          "name": "getGroups",
          "request": {
            "url": "http://apiv2.clickmeter.com:80/groups?createdAfter=%7B%7D&createdBefore=%7B%7D&limit=%7B%7D&offset=%7B%7D&status=%7B%7D&tags=%7B%7D&textSearch=%7B%7D&write=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of all the groups associated to the user.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da63ef9f-16c3-45d0-8b6d-e2471b0eae6d"
            }
          ]
        }
      ]
    }
  ]
}