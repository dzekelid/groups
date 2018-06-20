---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Delete an outcome group
  description: Delete an outcome group.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/assignment_groups:
    get:
      summary: List assignment groups
      description: List assignment groups.
      operationId: list-assignment-groups
      x-api-path-slug: coursescourse-idassignment-groups-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods feature turned on
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      - in: query
        name: scope_assignments_to_student
        description: If true, all assignments returned will apply to the current user
          in thenspecified grading period
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
    post:
      summary: Create an Assignment Group
      description: Create an assignment group.
      operationId: create-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groups-post
      parameters:
      - in: query
        name: group_weight
        description: The percent of the total grade that this assignment group represents
      - in: query
        name: name
        description: The assignment group&#39;s name
      - in: query
        name: position
        description: The position of this assignment group in relation to the other
          assignmentngroups
      - in: query
        name: rules
        description: The grading rules that are applied within this assignment group
          See thenAssignment Group object definition for format
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
  /courses/{course_id}/assignment_groups/assignment_group_id:
    delete:
      summary: Destroy an Assignment Group
      description: Destroy an assignment group.
      operationId: destroy-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-delete
      parameters:
      - in: query
        name: move_assignments_to
        description: The ID of an active Assignment Group to which the assignments
          that arencurrently assigned to the destroyed Assignment Group will be assigned
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    get:
      summary: Get an Assignment Group
      description: Get an assignment group.
      operationId: get-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods account feature turned
          on)
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    put:
      summary: Edit an Assignment Group
      description: Edit an assignment group.
      operationId: edit-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
  /courses/{course_id}/groups:
    get:
      summary: List the groups available in a context.
      description: List the groups available in a context..
      operationId: list-the-groups-available-in-a-context
      x-api-path-slug: coursescourse-idgroups-get
      parameters:
      - in: query
        name: only_own_groups
        description: Will only include groups that the user belongs to if this is
          set
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Groups
  /courses/{course_id}/outcome_groups:
    get:
      summary: Get all outcome groups for context
      description: Get all outcome groups for context.
      operationId: get-all-outcome-groups-for-context
      x-api-path-slug: coursescourse-idoutcome-groups-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
  /courses/{course_id}/outcome_groups/id:
    delete:
      summary: Delete an outcome group
      description: Delete an outcome group.
      operationId: delete-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---