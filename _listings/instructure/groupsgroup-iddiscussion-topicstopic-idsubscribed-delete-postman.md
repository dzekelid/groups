{
  "info": {
    "name": "Instructure Canvas Groups API Unsubscribe from a topic",
    "_postman_id": "549586dc-d211-4e0e-aa12-9a959eee297a",
    "description": "Unsubscribe from a topic.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "c0a03adf-f015-4a64-94ff-f871aa3173f9",
          "name": "create-a-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/groups?description=%7B%7D&is_public=%7B%7D&join_level=%7B%7D&name=%7B%7D&storage_quota_mb=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b282c0c-704f-41a0-b4b3-0a14063d51e3"
            }
          ]
        },
        {
          "id": "bc69da9c-43ce-497b-bce6-cfe60e18188c",
          "name": "get-a-single-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
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
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35123af2-a0f5-4eb9-bad1-e8042c9a056b"
            }
          ]
        },
        {
          "id": "81c33277-6982-46be-87e4-8117df9a5234",
          "name": "edit-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "avatar_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "join_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "members",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "storage_quota_mb",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53ca4fa8-4883-4c4c-ae6b-3719dbcf0031"
            }
          ]
        },
        {
          "id": "1bf4d287-d120-41b3-8ce8-b7a7dd6c6cff",
          "name": "delete-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac9c3018-b381-46a4-a30f-96453fd47ec1"
            }
          ]
        },
        {
          "id": "6f95c2b4-5313-498f-824a-97e7e39ab6c5",
          "name": "group-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10108d45-56ba-4b75-921a-a4b2d063cb15"
            }
          ]
        },
        {
          "id": "bf2c8adc-318c-4a47-8454-259794f983cc",
          "name": "group-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream/summary"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Group activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c23cf0f8-d268-4e34-89de-0375bd92b9b4"
            }
          ]
        },
        {
          "id": "25bdbec6-847a-4f93-8ec0-3f03ea6e300e",
          "name": "redirect-to-the-assignment-override-for-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "740c90b2-f803-4473-a7f0-ce020430e253"
            }
          ]
        },
        {
          "id": "da2f89e7-19ed-4b88-a5b8-d7d40ef36db1",
          "name": "list-conferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/conferences"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List conferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c188065-fada-4bc7-a496-76e81ecf6ed9"
            }
          ]
        },
        {
          "id": "e87ca870-a18c-4a49-971d-d20a63ba8014",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf873855-48fa-4bfb-8f7f-5cbe29f11d98"
            }
          ]
        },
        {
          "id": "a2546277-cd0f-4b99-a58e-3c9939d9ce7e",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
              ],
              "query": [
                {
                  "key": "export_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_notifications",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Export content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00f5a7f8-4d77-4062-bf88-4837fe1c6020"
            }
          ]
        },
        {
          "id": "c5c38faa-599b-4ff9-894c-d1d9f993e2ae",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1493a928-29c2-443b-aaa6-65b6716087b1"
            }
          ]
        },
        {
          "id": "8b64b33d-033d-4e30-bf7d-fba6d1d81804",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_licenses"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4d9649b-29b7-476d-b3a5-0d19fff28b38"
            }
          ]
        },
        {
          "id": "2f2fbcea-615d-496e-9d26-69036e9918ad",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "730a8ee2-b537-4361-929b-6c5af77af26a"
            }
          ]
        },
        {
          "id": "0143429c-7ecb-4626-a3db-cc004808beed",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
              ],
              "query": [
                {
                  "key": "date_shift_options[day_substitutions][X]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[remove_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[shift_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "migration_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[*]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[file_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[folder_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[overwrite_quizzes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[source_course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aea071d4-2b44-4d69-8a01-b8b3debbab38"
            }
          ]
        },
        {
          "id": "1ef13de2-36dd-453c-8757-0a398d41fd2b",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14acfd39-f365-472e-8ddf-8f4c8085c957"
            }
          ]
        },
        {
          "id": "c7de6cf0-f926-49df-8f0a-904136d4694f",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
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
            "description": "Get a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec425162-d823-4da1-9fd6-f847948af828"
            }
          ]
        },
        {
          "id": "a7a748b8-4b1a-4544-b4cf-160579c4b3db",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "query": [
                {
                  "key": "workflow_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
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
            "description": "Update a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ee6e23d-57cd-44b1-90a4-8371c9d18153"
            }
          ]
        },
        {
          "id": "608318fd-a035-4060-9f0a-89ceec2c0d67",
          "name": "get-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3e04235-f129-4cf1-8b46-d917dcf0d333"
            }
          ]
        },
        {
          "id": "a1fb5106-901d-44be-b352-9e283e49e183",
          "name": "update-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fd63e1f-090c-4755-878c-b476bab1ba47"
            }
          ]
        },
        {
          "id": "c9c9f113-387d-4603-89dd-5b6230001bc4",
          "name": "list-migration-systems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/migrators"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration systems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70be3a83-dd44-46a4-8b2d-2325698d7c1c"
            }
          ]
        },
        {
          "id": "defb422f-8dcc-4e99-9da6-7ff4551eae40",
          "name": "list-discussion-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "only_announcements",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List discussion topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e927d00a-75f2-4e3d-b10b-50b62d7f891a"
            }
          ]
        },
        {
          "id": "0496975b-c8c0-4fa2-96f9-341afdb074c5",
          "name": "create-a-new-discussion-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new discussion topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a1f0fde-9252-42b8-ad5c-e9fb67b9de08"
            }
          ]
        },
        {
          "id": "758e02ab-e4a7-4da8-a557-ad5ac9cb588d",
          "name": "reorder-pinned-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/reorder"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder pinned topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67f49277-6f66-45fb-a3fe-0397e98a6ecf"
            }
          ]
        },
        {
          "id": "e7177284-5a4f-43d9-bed5-9e2af3315d71",
          "name": "get-a-single-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c68a79ff-4488-4fa2-a910-139a9a7cee16"
            }
          ]
        },
        {
          "id": "1313bff9-7a1c-4362-8b08-9d5e6f6fc0ef",
          "name": "update-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb99f88a-5a94-42be-b9b5-f98f383391c6"
            }
          ]
        },
        {
          "id": "6358b2f7-ac80-4d7d-9a0c-39fb0c15dbd4",
          "name": "delete-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1656673-34ec-4d61-aef3-ea96146e29f4"
            }
          ]
        },
        {
          "id": "438e9efb-191b-4584-a3cf-e544ebbfd3a1",
          "name": "list-topic-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List topic entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2377c611-be9c-4c3c-b5ba-ddcc56135498"
            }
          ]
        },
        {
          "id": "b1bcba59-2f42-4048-b983-87ac6759c384",
          "name": "post-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14c1c4ab-dfdc-41ff-9504-e1363b4c3a94"
            }
          ]
        },
        {
          "id": "4b4f7e46-1c38-4376-923d-22405adc7093",
          "name": "rate-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/rating"
              ],
              "query": [
                {
                  "key": "rating",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rate entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4dbf264-9106-4da4-9fd1-1e06a81d56c5"
            }
          ]
        },
        {
          "id": "e865cf17-5f3e-4c46-8922-e54ccdb83ab2",
          "name": "mark-entry-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd4e1de2-8265-4f5f-90ad-8adc10abaca7"
            }
          ]
        },
        {
          "id": "35aea717-aaa7-40ee-af92-bf503b393084",
          "name": "mark-entry-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd1d3203-8a95-4224-abf5-1e6db03845b7"
            }
          ]
        },
        {
          "id": "dd5e32f0-bd9f-49f4-b21f-0904f7018b5c",
          "name": "list-entry-replies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entry replies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5b90ae2-2e3d-4ee0-bf32-afad1c07c183"
            }
          ]
        },
        {
          "id": "40119771-f755-4200-a289-49cc521d08b2",
          "name": "post-a-reply",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post a reply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efb05733-9163-4f5e-8589-ce7f41e26775"
            }
          ]
        },
        {
          "id": "4433f37c-b400-4517-897e-4dfbb268646d",
          "name": "update-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
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
            "description": "Update an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1617b596-0839-4a17-9989-a0a964b46413"
            }
          ]
        },
        {
          "id": "0e8ee265-8365-43be-9e27-6cceefb83e1b",
          "name": "delete-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
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
            "description": "Delete an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38ffdd97-a056-4046-bda3-a2dddd5d02ef"
            }
          ]
        },
        {
          "id": "ebf6d2db-f00b-42e1-89c3-2dbc7ef3f659",
          "name": "list-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entry_list"
              ],
              "query": [
                {
                  "key": "ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e617b5b0-e3b3-4caf-bbc6-6b4a0d8bfdb6"
            }
          ]
        },
        {
          "id": "5a431be8-e485-449d-bc2d-3cc6ac5396b3",
          "name": "mark-topic-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark topic as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2612cc84-fa0f-42a5-bf23-f8ceea94355a"
            }
          ]
        },
        {
          "id": "0b1d7a30-6813-472e-b0ce-d767874e0a3c",
          "name": "mark-topic-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark topic as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40b1c756-8437-44af-9c9c-ba18921d64ae"
            }
          ]
        },
        {
          "id": "d89e4415-3ae1-4cfe-9c6f-9e0ed923865b",
          "name": "mark-all-entries-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28ba4900-c313-478f-8c0b-6991e71c605c"
            }
          ]
        },
        {
          "id": "73e986e8-f9b8-4321-90d8-eaeab0643b69",
          "name": "mark-all-entries-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0394967f-8e41-40d8-a2b4-cd3001b515a6"
            }
          ]
        },
        {
          "id": "29888a1a-c12c-4683-92aa-2b31936dcc01",
          "name": "unsubscribe-from-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unsubscribe from a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "833f41f8-7800-4db5-839b-80a03942a0ea"
            }
          ]
        }
      ]
    }
  ]
}