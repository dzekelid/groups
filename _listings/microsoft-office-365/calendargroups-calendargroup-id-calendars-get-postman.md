{
  "info": {
    "name": "Microsoft Office 365 Get Calendar Groups Calendars",
    "_postman_id": "0a4e911d-a55f-427c-bb5a-33fbe5d2b1fd",
    "description": "You can request all the user's calendars (or a filtered list...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendargroups",
      "item": [
        {
          "id": "70708098-151e-4b2a-b97a-821eeb8d542d",
          "name": "getCalendargroupsCalendargroupCalendars",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "CalendarGroups:calendargroup_id/Calendars"
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
            "description": "You can request all the user's calendars (or a filtered list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adb34f9b-9f5d-4f4d-ab51-6965c18ae05e"
            }
          ]
        }
      ]
    }
  ]
}