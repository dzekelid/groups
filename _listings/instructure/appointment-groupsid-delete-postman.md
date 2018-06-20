{
  "info": {
    "name": "Instructure Canvas Appointment Groups API Delete an appointment group",
    "_postman_id": "e4e5e8f8-e83e-4189-a3df-9096df07393c",
    "description": "Delete an appointment group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "0778f466-6c66-4a48-b3e1-eb3914ed9008",
          "name": "list-appointment-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?context_codes=%5B%7B%7D%5D&include=%5B%7B%7D%5D&include_past_appointments=%7B%7D&scope=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List appointment groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea1efa7a-5114-4e30-8ee6-df9fa00ac209"
            }
          ]
        },
        {
          "id": "80dd8976-4630-43c0-84c3-532fbc284bcc",
          "name": "create-an-appointment-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?appointment_group[context_codes=%5B%7B%7D%5D&appointment_group[description]=%7B%7D&appointment_group[location_address]=%7B%7D&appointment_group[location_name]=%7B%7D&appointment_group[max_appointments_per_participant]=%7B%7D&appointment_group[min_appointments_per_participant]=%7B%7D&appointment_group[new_appointments][X=%5B%7B%7D%5D&appointment_group[participants_per_appointment]=%7B%7D&appointment_group[participant_visibility]=%7B%7D&appointment_group[publish]=%7B%7D&appointment_group[sub_context_codes=%5B%7B%7D%5D&appointment_group[title]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18f5cd77-7fbe-4d98-9b28-2cbc9229fde4"
            }
          ]
        },
        {
          "id": "783f60b5-1a4c-49b9-ba75-1dfa73ab032c",
          "name": "delete-an-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "cancel_reason",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bcf8f991-77e3-43e2-b3e8-5851a6196ed9"
            }
          ]
        }
      ]
    }
  ]
}