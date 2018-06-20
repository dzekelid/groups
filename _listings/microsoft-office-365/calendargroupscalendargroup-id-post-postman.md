{
  "info": {
    "name": "Microsoft Office 365 Add Calendar Groups",
    "_postman_id": "e9899759-f410-460e-951b-28c6496ac54e",
    "description": "Post calendargroups calendargroup",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendargroups",
      "item": [
        {
          "id": "09390c19-eb2d-4445-9c32-74217859aeb5",
          "name": "postCalendargroupsCalendargroup",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post calendargroups calendargroup"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1586398-d0d2-4c85-ad6d-97bde0539979"
            }
          ]
        }
      ]
    }
  ]
}