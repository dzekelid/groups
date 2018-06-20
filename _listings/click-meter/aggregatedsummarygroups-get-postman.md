{
  "info": {
    "name": "Click Meter Retrieve statistics about a subset of groups for a timeframe with groups data",
    "_postman_id": "86ab4b9b-dad3-45d4-8dbf-c926f0ec7165",
    "description": "Retrieve statistics about a subset of groups for a timeframe with groups data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Aggregated",
      "item": [
        {
          "id": "2d07c185-fcb8-46b4-add7-8fe1d3621cde",
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
              "id": "c750e6c0-b3d1-4817-9bee-da911d456f02"
            }
          ]
        }
      ]
    }
  ]
}