{
  "info": {
    "name": "Microsoft Office 365 Get Calendar Groups",
    "_postman_id": "7f68a383-f4d5-41b8-bdc1-d87397ce34e0",
    "description": "You can request all the calendar groups in a mailbox (or a f...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendargroups",
      "item": [
        {
          "id": "b13c12c5-548b-4849-987c-690bf340b4ed",
          "name": "getCalendargroups",
          "request": {
            "url": "http://outlook.office365.com/ews/odata/Me/CalendarGroups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can request all the calendar groups in a mailbox (or a f"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12212781-e2e4-44bb-89ba-b3395c652fd6"
            }
          ]
        }
      ]
    }
  ]
}