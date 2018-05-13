{
  "info": {
    "name": "Microsoft Office 365 Delete Calendar Groups",
    "_postman_id": "fab49ecc-7877-42ee-8496-b0ce9ff68988",
    "description": "Deleting a calendar group is as simple as sending a DELETE r...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendargroups",
      "item": [
        {
          "id": "ddffe21b-4bd6-4225-84e6-c42dd51ea959",
          "name": "deleteCalendargroupsCalendargroup",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deleting a calendar group is as simple as sending a DELETE r"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0411ef58-3ca3-4472-908f-d3406d635717"
            }
          ]
        }
      ]
    }
  ]
}