---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Create a subgroup
  description: Create a subgroup.
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
  /appointment_groups:
    get:
      summary: List appointment groups
      description: List appointment groups.
      operationId: list-appointment-groups
      x-api-path-slug: appointment-groups-get
      parameters:
      - in: query
        name: context_codes[]
        description: Array of context codes used to limit returned results
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: include_past_appointments
        description: Defaults to false
      - in: query
        name: scope
        description: 'Defaults to u201creservableu201dnn        n        n          Allowed
          values: reservable, manageable'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
    post:
      summary: Create an appointment group
      description: Create an appointment group.
      operationId: create-an-appointment-group
      x-api-path-slug: appointment-groups-post
      parameters:
      - in: query
        name: appointment_group[context_codes][]
        description: Array of context codes (courses, e
      - in: query
        name: appointment_group[description]
        description: Longer text description of the appointment group
      - in: query
        name: appointment_group[location_address]
        description: Location address
      - in: query
        name: appointment_group[location_name]
        description: Location name of the appointment group
      - in: query
        name: appointment_group[max_appointments_per_participant]
        description: Maximum number of time slots a user may register for
      - in: query
        name: appointment_group[min_appointments_per_participant]
        description: Minimum number of time slots a user must register for
      - in: query
        name: appointment_group[new_appointments][X][]
        description: Nested array of start time/end time pairs indicating time slots
          for thisnappointment group
      - in: query
        name: appointment_group[participants_per_appointment]
        description: Maximum number of participants that may register for each time
          slot
      - in: query
        name: appointment_group[participant_visibility]
        description: u201cprivateu201dnnparticipants cannot see who has signed up
          for a particular time slotnu201cprotectedu201dnnparticipants can see who
          has signed up
      - in: query
        name: appointment_group[publish]
        description: Indicates whether this appointment group should be published
          (i
      - in: query
        name: appointment_group[sub_context_codes][]
        description: Array of sub context codes (course sections or a single group
          category)nthis group should be linked to
      - in: query
        name: appointment_group[title]
        description: Short title for the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
  /appointment_groups/{id}:
    delete:
      summary: Delete an appointment group
      description: Delete an appointment group.
      operationId: delete-an-appointment-group
      x-api-path-slug: appointment-groupsid-delete
      parameters:
      - in: query
        name: cancel_reason
        description: Reason for deleting/canceling the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
    get:
      summary: Get a single appointment group
      description: Get a single appointment group.
      operationId: get-a-single-appointment-group
      x-api-path-slug: appointment-groupsid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
    put:
      summary: Update an appointment group
      description: Update an appointment group.
      operationId: update-an-appointment-group
      x-api-path-slug: appointment-groupsid-put
      parameters:
      - in: query
        name: appointment_group[context_codes][]
        description: Array of context codes (courses, e
      - in: query
        name: appointment_group[description]
        description: Longer text description of the appointment group
      - in: query
        name: appointment_group[location_address]
        description: Location address
      - in: query
        name: appointment_group[location_name]
        description: Location name of the appointment group
      - in: query
        name: appointment_group[max_appointments_per_participant]
        description: Maximum number of time slots a user may register for
      - in: query
        name: appointment_group[min_appointments_per_participant]
        description: Minimum number of time slots a user must register for
      - in: query
        name: appointment_group[new_appointments][X][]
        description: Nested array of start time/end time pairs indicating time slots
          for thisnappointment group
      - in: query
        name: appointment_group[participants_per_appointment]
        description: Maximum number of participants that may register for each time
          slot
      - in: query
        name: appointment_group[participant_visibility]
        description: u201cprivateu201dnnparticipants cannot see who has signed up
          for a particular time slotnu201cprotectedu201dnnparticipants can see who
          has signed up
      - in: query
        name: appointment_group[publish]
        description: Indicates whether this appointment group should be published
          (i
      - in: query
        name: appointment_group[sub_context_codes][]
        description: Array of sub context codes (course sections or a single group
          category)nthis group should be linked to
      - in: query
        name: appointment_group[title]
        description: Short title for the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
  /appointment_groups/{id}/groups:
    get:
      summary: List student group participants
      description: List student group participants.
      operationId: list-student-group-participants
      x-api-path-slug: appointment-groupsidgroups-get
      parameters:
      - in: query
        name: registration_status
        description: 'Limits results to the a given participation status, defaults
          to u201callu201dnn        n        n          Allowed values: all, registered,
          registered'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
      - Groups
  /appointment_groups/{id}/users:
    get:
      summary: List user participants
      description: List user participants.
      operationId: list-user-participants
      x-api-path-slug: appointment-groupsidusers-get
      parameters:
      - in: query
        name: registration_status
        description: 'Limits results to the a given participation status, defaults
          to u201callu201dnn        n        n          Allowed values: all, registered,
          registered'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
      - Users
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
    get:
      summary: Show an outcome group
      description: Show an outcome group.
      operationId: show-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-get
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
    put:
      summary: Update an outcome group
      description: Update an outcome group.
      operationId: update-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-put
      parameters:
      - in: query
        name: description
        description: The new outcome group description
      - in: query
        name: parent_outcome_group_id
        description: The id of the new parent outcome group
      - in: query
        name: title
        description: The new outcome group title
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
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
  /courses/{course_id}/outcome_groups/id/import:
    post:
      summary: Import an outcome group
      description: Import an outcome group.
      operationId: import-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsidimport-post
      parameters:
      - in: query
        name: source_outcome_group_id
        description: The ID of the source outcome group
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
      - Import
  /courses/{course_id}/outcome_groups/id/outcomes:
    get:
      summary: List linked outcomes
      description: List linked outcomes.
      operationId: list-linked-outcomes
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-get
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
      - Outcomes
    post:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-post
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The description of the new outcome
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The mastery threshold for the embedded rubric criterion
      - in: query
        name: outcome_id
        description: The ID of the existing outcome to link
      - in: query
        name: ratings[][description]
        description: The description of a rating level for the embedded rubric criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a rating level for the embedded rubricncriterion
      - in: query
        name: title
        description: The title of the new outcome
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
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
      - Outcomes
  /courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}:
    delete:
      summary: Unlink an outcome
      description: Unlink an outcome.
      operationId: unlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete
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
      - Outcomes
      - Outcome
      - Id
    put:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-put
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The description of the new outcome
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The mastery threshold for the embedded rubric criterion
      - in: query
        name: outcome_id
        description: The ID of the existing outcome to link
      - in: query
        name: ratings[][description]
        description: The description of a rating level for the embedded rubric criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a rating level for the embedded rubricncriterion
      - in: query
        name: title
        description: The title of the new outcome
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
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
      - Outcomes
      - Outcome
      - Id
  /courses/{course_id}/outcome_groups/id/subgroups:
    get:
      summary: List subgroups
      description: List subgroups.
      operationId: list-subgroups
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-get
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
      - Subgroups
    post:
      summary: Create a subgroup
      description: Create a subgroup.
      operationId: create-a-subgroup
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-post
      parameters:
      - in: query
        name: description
        description: The description of the new outcome group
      - in: query
        name: title
        description: The title of the new outcome group
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
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
      - Subgroups
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