{
  "info": {
    "name": "Microsoft Office 365 Get Calendar Groups",
    "_postman_id": "40ac0866-526e-483d-8d67-c82663fdc194",
    "description": "Get calendargroups calendargroup",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendargroups",
      "item": [
        {
          "id": "3c78fc85-4d0f-40fa-a811-0b24bbdac651",
          "name": "getCalendargroupsCalendargroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "CalendarGroups:calendargroup_id"
              ],
              "variable": [
                {
                  "id": "calendargroup_id",
                  "value": "calendargroup_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get calendargroups calendargroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "622ff82d-d425-42e6-8dc3-06a7fb292d54"
            }
          ]
        }
      ]
    }
  ]
}