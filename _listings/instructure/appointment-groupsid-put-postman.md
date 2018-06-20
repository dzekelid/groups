{
  "info": {
    "name": "Instructure Canvas Appointment Groups API Update an appointment group",
    "_postman_id": "b3ed36c0-b679-4d8b-97a3-84200942603e",
    "description": "Update an appointment group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "96e647d1-2ed9-420d-9a98-06857b053056",
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
              "id": "97483e12-cfad-4667-bdb2-377f3f3abb6e"
            }
          ]
        },
        {
          "id": "f3d76615-2c14-4139-b26e-4af646911bf9",
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
              "id": "016aba10-c12d-47d6-9ca8-87d2f765d64a"
            }
          ]
        },
        {
          "id": "1af97cfd-7843-4192-8cdc-88b9e4dbff1d",
          "name": "get-a-single-appointment-group",
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
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37449356-15e4-404c-9fe5-59275eca49d0"
            }
          ]
        },
        {
          "id": "60d08bc4-cca1-4a3f-851a-91c9edb79006",
          "name": "update-an-appointment-group",
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
                  "key": "appointment_group[context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[max_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[min_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[new_appointments][X",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participants_per_appointment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participant_visibility]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[publish]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[sub_context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[title]",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "950268ac-6bd7-4d9b-ba0a-c8c7861436ef"
            }
          ]
        },
        {
          "id": "ba3f2a37-cc34-43e8-865d-f692768c88d4",
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
              "id": "8999f32b-e5d2-49e1-82a9-faa1db6d6ad4"
            }
          ]
        }
      ]
    }
  ]
}