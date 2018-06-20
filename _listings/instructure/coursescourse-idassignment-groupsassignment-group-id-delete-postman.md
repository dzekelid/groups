{
  "info": {
    "name": "Instructure Canvas Courses API Destroy an Assignment Group",
    "_postman_id": "0fa5acc9-55cc-45e1-b3d8-73bdf17ddf49",
    "description": "Destroy an assignment group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Courses",
      "item": [
        {
          "id": "cf9ba882-c869-4ef0-ab29-b7a3678a84c0",
          "name": "list-assignment-groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups"
              ],
              "query": [
                {
                  "key": "grading_period_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "override_assignment_dates",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope_assignments_to_student",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List assignment groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c72085e-2d76-471b-b893-50e8f647100e"
            }
          ]
        },
        {
          "id": "41a51f96-519c-41d7-94ec-488504fbfcc6",
          "name": "create-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups"
              ],
              "query": [
                {
                  "key": "group_weight",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "rules",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e913b607-8739-44b5-8e11-407ab0038b20"
            }
          ]
        },
        {
          "id": "ad7e8e49-f4ba-4c2a-9e06-f0e0d1bff53e",
          "name": "destroy-an-assignment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "courses/:course_id/assignment_groups/assignment_group_id"
              ],
              "query": [
                {
                  "key": "move_assignments_to",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Destroy an assignment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35cf8dc8-e6e6-4a2b-a8cc-59323a93839b"
            }
          ]
        }
      ]
    }
  ]
}