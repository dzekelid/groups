{
  "info": {
    "name": "Clarity Accounting Delete Contact Groups Contacts",
    "_postman_id": "31ad1566-dab9-429c-9170-dd2366a35d16",
    "description": "Delete contactgroups contactgroup contacts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "ContactGroups",
      "item": [
        {
          "id": "52b58fd9-715d-4412-a812-a6ba6b90da32",
          "name": "deleteContactgroupsContactgroupContacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.xero.com",
              "path": [
                "api.xro",
                "2.0",
                "ContactGroups/:ContactGroupID/Contacts"
              ],
              "variable": [
                {
                  "id": "ContactGroupID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete contactgroups contactgroup contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7de1ea44-0479-426d-95ce-61a5c51ff9ed"
            }
          ]
        }
      ]
    }
  ]
}