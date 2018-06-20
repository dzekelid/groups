{
  "info": {
    "name": "Instructure Canvas Appointment Groups API List student group participants",
    "_postman_id": "775c662c-97ee-4f51-b280-a820bc0e576a",
    "description": "List student group participants.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "1b170f53-4af5-44de-af6b-27432bb10019",
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
              "id": "2b2e92c7-a2e7-4f63-9460-8caf565e1951"
            }
          ]
        },
        {
          "id": "764aba3c-8cad-4e78-8f2e-fc292f6be8cc",
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
              "id": "8e5f954b-88bc-4603-8127-8b6ba0abac41"
            }
          ]
        },
        {
          "id": "bd519368-d5de-4f8d-9b90-362d156750b3",
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
              "id": "e71c987d-c6d4-4fb1-aeaf-231727feab2d"
            }
          ]
        },
        {
          "id": "04788011-79fc-405f-b308-de17611894d3",
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
              "id": "4f59e00c-f7f4-4c5f-b516-041fa703da9a"
            }
          ]
        },
        {
          "id": "0a4792b3-063a-4a4b-a4e8-fe8333bcc45f",
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
              "id": "90cbc3ee-b500-4ad9-84c2-d4ad32470ac0"
            }
          ]
        },
        {
          "id": "70186753-caf4-4640-be9b-5f0fceae57fe",
          "name": "list-student-group-participants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id/groups"
              ],
              "query": [
                {
                  "key": "registration_status",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List student group participants."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07fd1b38-bd1d-4024-91a0-79550eb91c6c"
            }
          ]
        }
      ]
    }
  ]
}