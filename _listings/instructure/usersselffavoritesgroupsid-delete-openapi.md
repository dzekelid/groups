---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Remove group from favorites
  description: Remove group from favorites.
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
  /courses/{course_id}/quizzes/quiz_id/groups:
    post:
      summary: Create a question group
      description: Create a question group.
      operationId: create-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroups-post
      parameters:
      - in: query
        name: quiz_groups[][assessment_question_bank_id]
        description: The id of the assessment question bank to pull questions from
      - in: query
        name: quiz_groups[][name]
        description: The name of the question group
      - in: query
        name: quiz_groups[][pick_count]
        description: The number of questions to randomly select for this group
      - in: query
        name: quiz_groups[][question_points]
        description: The number of points to assign to each question in the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
  /courses/{course_id}/quizzes/quiz_id/groups/{id}:
    delete:
      summary: Delete a question group
      description: Delete a question group.
      operationId: delete-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
    get:
      summary: Get a single quiz group
      description: Get a single quiz group.
      operationId: get-a-single-quiz-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
    put:
      summary: Update a question group
      description: Update a question group.
      operationId: update-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-put
      parameters:
      - in: query
        name: quiz_groups[][name]
        description: The name of the question group
      - in: query
        name: quiz_groups[][pick_count]
        description: The number of questions to randomly select for this group
      - in: query
        name: quiz_groups[][question_points]
        description: The number of points to assign to each question in the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
  /courses/{course_id}/quizzes/quiz_id/groups/{id}/reorder:
    post:
      summary: Reorder question groups
      description: Reorder question groups.
      operationId: reorder-question-groups
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsidreorder-post
      parameters:
      - in: query
        name: order[][id]
        description: The associated item&#39;s unique identifier
      - in: query
        name: order[][type]
        description: 'The type of item is always &#39;question&#39; for a groupnn        n        n          Allowed
          values: question'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
      - Reorder
  /courses/{course_id}/group_categories:
    get:
      summary: List group categories for a context
      description: List group categories for a context.
      operationId: list-group-categories-for-a-context
      x-api-path-slug: coursescourse-idgroup-categories-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
      - Categories
    post:
      summary: Create a Group Category
      description: Create a group category.
      operationId: create-a-group-category
      x-api-path-slug: coursescourse-idgroup-categories-post
      parameters:
      - in: query
        name: auto_leader
        description: 'Assigns group leaders automatically when generating and allocating
          studentsnto groups Valid values are:nu201cfirstu201dnnthe first student
          to be allocated to a group is the leadernu201crandomu201dnna random student
          from all members is chosen as the leadernnn        n        n          Allowed
          values: first, random'
      - in: query
        name: create_group_count
        description: Create this number of groups (Course Only)
      - in: query
        name: group_limit
        description: Limit the maximum number of users in each group (Course Only)
      - in: query
        name: name
        description: Name of the group category
      - in: query
        name: self_signup
        description: Allow students to sign up for a group themselves (Course Only)
      - in: query
        name: split_group_count
        description: (Deprecated) Create this number of groups, and evenly distribute
          studentsnamong them
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
      - Categories
  /courses/{course_id}/outcome_group_links:
    get:
      summary: Get all outcome links for context
      description: Get all outcome links for context.
      operationId: get-all-outcome-links-for-context
      x-api-path-slug: coursescourse-idoutcome-group-links-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Group
      - Links
  /courses/{course_id}/root_outcome_group:
    get:
      summary: Redirect to root outcome group for context
      description: Redirect to root outcome group for context.
      operationId: redirect-to-root-outcome-group-for-context
      x-api-path-slug: coursescourse-idroot-outcome-group-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Root
      - Outcome
      - Group
  /global/outcome_groups/{id}:
    delete:
      summary: Delete an outcome group
      description: Delete an outcome group.
      operationId: delete-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
    get:
      summary: Show an outcome group
      description: Show an outcome group.
      operationId: show-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
    put:
      summary: Update an outcome group
      description: Update an outcome group.
      operationId: update-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-put
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
      - Global
      - Outcome
      - Groups
      - Id
  /global/outcome_groups/{id}/import:
    post:
      summary: Import an outcome group
      description: Import an outcome group.
      operationId: import-an-outcome-group
      x-api-path-slug: globaloutcome-groupsidimport-post
      parameters:
      - in: query
        name: source_outcome_group_id
        description: The ID of the source outcome group
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Import
  /global/outcome_groups/{id}/outcomes:
    get:
      summary: List linked outcomes
      description: List linked outcomes.
      operationId: list-linked-outcomes
      x-api-path-slug: globaloutcome-groupsidoutcomes-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Outcomes
    post:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: globaloutcome-groupsidoutcomes-post
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
      - Global
      - Outcome
      - Groups
      - Id
      - Outcomes
  /global/outcome_groups/{id}/outcomes/outcome_id:
    delete:
      summary: Unlink an outcome
      description: Unlink an outcome.
      operationId: unlink-an-outcome
      x-api-path-slug: globaloutcome-groupsidoutcomesoutcome-id-delete
      responses:
        200:
          description: OK
      tags:
      - Global
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
      x-api-path-slug: globaloutcome-groupsidoutcomesoutcome-id-put
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
      - Global
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
      - Id
  /global/outcome_groups/{id}/subgroups:
    get:
      summary: List subgroups
      description: List subgroups.
      operationId: list-subgroups
      x-api-path-slug: globaloutcome-groupsidsubgroups-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Subgroups
    post:
      summary: Create a subgroup
      description: Create a subgroup.
      operationId: create-a-subgroup
      x-api-path-slug: globaloutcome-groupsidsubgroups-post
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
      - Global
      - Outcome
      - Groups
      - Id
      - Subgroups
  /global/root_outcome_group:
    get:
      summary: Redirect to root outcome group for context
      description: Redirect to root outcome group for context.
      operationId: redirect-to-root-outcome-group-for-context
      x-api-path-slug: globalroot-outcome-group-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Root
      - Outcome
      - Group
  /groups:
    post:
      summary: Create a group
      description: Create a group.
      operationId: create-a-group
      x-api-path-slug: groups-post
      parameters:
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}:
    delete:
      summary: Delete a group
      description: Delete a group.
      operationId: delete-a-group
      x-api-path-slug: groupsgroup-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    get:
      summary: Get a single group
      description: Get a single group.
      operationId: get-a-single-group
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cpermissionsu201d: Include permissions the current user
          has for the group'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    put:
      summary: Edit a group
      description: Edit a group.
      operationId: edit-a-group
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: query
        name: avatar_id
        description: The id of the attachment previously uploaded to the group that
          you wouldnlike to use as the avatar image for this group
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: Whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: members[]
        description: An array of user ids for users you would like in the group
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
  /groups/{group_id}/activity_stream:
    get:
      summary: Group activity stream
      description: Group activity stream.
      operationId: group-activity-stream
      x-api-path-slug: groupsgroup-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
  /groups/{group_id}/activity_stream/summary:
    get:
      summary: Group activity stream summary
      description: Group activity stream summary.
      operationId: group-activity-stream-summary
      x-api-path-slug: groupsgroup-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
      - Summary
  /groups/{group_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a group
      description: Redirect to the assignment override for a group.
      operationId: redirect-to-the-assignment-override-for-a-group
      x-api-path-slug: groupsgroup-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /groups/{group_id}/conferences:
    get:
      summary: List conferences
      description: List conferences.
      operationId: list-conferences
      x-api-path-slug: groupsgroup-idconferences-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Conferences
  /groups/{group_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: groupsgroup-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: groupsgroup-idcontent-exports-post
      parameters:
      - in: query
        name: export_type
        description: u201ccommon_cartridgeu201dnnExport the contents of the course
          in the Common Cartridge (
      - in: query
        name: skip_notifications
        description: Don&#39;t send the notifications about the export to the user
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
  /groups/{group_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: groupsgroup-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
      - Id
  /groups/{group_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: groupsgroup-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Licenses
  /groups/{group_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: groupsgroup-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
    post:
      summary: Create a content migration
      description: Create a content migration.
      operationId: create-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrations-post
      parameters:
      - in: query
        name: date_shift_options[day_substitutions][X]
        description: Move anything scheduled for day &#39;X&#39; to the specified
          day
      - in: query
        name: date_shift_options[new_end_date]
        description: The new end date for the source content/course
      - in: query
        name: date_shift_options[new_start_date]
        description: The new start date for the content/course
      - in: query
        name: date_shift_options[old_end_date]
        description: The original end date of the source content/course
      - in: query
        name: date_shift_options[old_start_date]
        description: The original start date of the source content/course
      - in: query
        name: date_shift_options[remove_dates]
        description: Whether to remove dates in the copied course
      - in: query
        name: date_shift_options[shift_dates]
        description: Whether to shift dates in the copied course
      - in: query
        name: migration_type
        description: The type of the migration
      - in: query
        name: pre_attachment[*]
        description: Other file upload properties, See File Upload Documentation
      - in: query
        name: pre_attachment[name]
        description: Required if uploading a file
      - in: query
        name: settings[file_url]
        description: A URL to download the file from
      - in: query
        name: settings[folder_id]
        description: 'The folder to unzip the '
      - in: query
        name: settings[overwrite_quizzes]
        description: Whether to overwrite quizzes with the same identifiers between
          contentnpackages
      - in: query
        name: settings[question_bank_id]
        description: The existing question bank ID to import questions into if not
          specified innthe content package
      - in: query
        name: settings[question_bank_name]
        description: The question bank to import questions into if not specified in
          the contentnpackage, if both bank id and name are set, id will take precedence
      - in: query
        name: settings[source_course_id]
        description: The course to copy from for a course copy migration
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues:
    get:
      summary: List migration issues
      description: List migration issues.
      operationId: list-migration-issues
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}:
    get:
      summary: Get a migration issue
      description: Get a migration issue.
      operationId: get-a-migration-issue
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
    put:
      summary: Update a migration issue
      description: Update a migration issue.
      operationId: update-a-migration-issue
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put
      parameters:
      - in: query
        name: workflow_state
        description: Set the workflow_state of the issue
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
  /groups/{group_id}/content_migrations/id:
    get:
      summary: Get a content migration
      description: Get a content migration.
      operationId: get-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
    put:
      summary: Update a content migration
      description: Update a content migration.
      operationId: update-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
  /groups/{group_id}/content_migrations/migrators:
    get:
      summary: List Migration Systems
      description: List migration systems.
      operationId: list-migration-systems
      x-api-path-slug: groupsgroup-idcontent-migrationsmigrators-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Migrators
  /groups/{group_id}/discussion_topics:
    get:
      summary: List discussion topics
      description: List discussion topics.
      operationId: list-discussion-topics
      x-api-path-slug: groupsgroup-iddiscussion-topics-get
      parameters:
      - in: query
        name: only_announcements
        description: Return announcements instead of discussion topics
      - in: query
        name: order_by
        description: Determines the order of the discussion topic list
      - in: query
        name: scope
        description: Only return discussion topics in the given state(s)
      - in: query
        name: search_term
        description: The partial title of the discussion topics to match and return
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
    post:
      summary: Create a new discussion topic
      description: Create a new discussion topic.
      operationId: create-a-new-discussion-topic
      x-api-path-slug: groupsgroup-iddiscussion-topics-post
      parameters:
      - in: query
        name: allow_rating
        description: If true, users will be allowed to rate entries
      - in: query
        name: assignment
        description: To create an assignment discussion, pass the assignment parameters
          as ansub-object
      - in: query
        name: attachment
        description: A multipart/form-data form-field-style attachment
      - in: query
        name: delayed_post_at
        description: If a timestamp is given, the topic will not be published until
          that time
      - in: query
        name: discussion_type
        description: The type of discussion
      - in: query
        name: group_category_id
        description: If present, the topic will become a group discussion assigned
          to the group
      - in: query
        name: is_announcement
        description: If true, this topic is an announcement
      - in: query
        name: lock_at
        description: If a timestamp is given, the topic will be scheduled to lock
          at thenprovided timestamp
      - in: query
        name: message
        description: no description
      - in: query
        name: only_graders_can_rate
        description: If true, only graders will be allowed to rate entries
      - in: query
        name: pinned
        description: If true, this topic will be listed in the u201cPinned Discussionu201d
          section
      - in: query
        name: podcast_enabled
        description: If true, the topic will have an associated podcast feed
      - in: query
        name: podcast_has_student_posts
        description: If true, the podcast will include posts from students as well
      - in: query
        name: position_after
        description: By default, discussions are sorted chronologically by creation
          date, youncan pass the id of another topic to have this one show up after
          the othernwhen they are listed
      - in: query
        name: published
        description: Whether this topic is published (true) or draft state (false)
      - in: query
        name: require_initial_post
        description: If true then a user may not respond to other replies until that
          user hasnmade an initial reply
      - in: query
        name: sort_by_rating
        description: If true, entries will be sorted by rating
      - in: query
        name: title
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
  /groups/{group_id}/discussion_topics/reorder:
    post:
      summary: Reorder pinned topics
      description: Reorder pinned topics.
      operationId: reorder-pinned-topics
      x-api-path-slug: groupsgroup-iddiscussion-topicsreorder-post
      parameters:
      - in: query
        name: order[]
        description: The ids of the pinned discussion topics in the desired order
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Reorder
  /groups/{group_id}/discussion_topics/topic_id:
    delete:
      summary: Delete a topic
      description: Delete a topic.
      operationId: delete-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    get:
      summary: Get a single topic
      description: Get a single topic.
      operationId: get-a-single-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    put:
      summary: Update a topic
      description: Update a topic.
      operationId: update-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-put
      parameters:
      - in: query
        name: allow_rating
        description: If true, users will be allowed to rate entries
      - in: query
        name: assignment
        description: To create an assignment discussion, pass the assignment parameters
          as ansub-object
      - in: query
        name: delayed_post_at
        description: If a timestamp is given, the topic will not be published until
          that time
      - in: query
        name: discussion_type
        description: The type of discussion
      - in: query
        name: group_category_id
        description: If present, the topic will become a group discussion assigned
          to the group
      - in: query
        name: is_announcement
        description: If true, this topic is an announcement
      - in: query
        name: lock_at
        description: If a timestamp is given, the topic will be scheduled to lock
          at thenprovided timestamp
      - in: query
        name: message
        description: no description
      - in: query
        name: only_graders_can_rate
        description: If true, only graders will be allowed to rate entries
      - in: query
        name: pinned
        description: If true, this topic will be listed in the u201cPinned Discussionu201d
          section
      - in: query
        name: podcast_enabled
        description: If true, the topic will have an associated podcast feed
      - in: query
        name: podcast_has_student_posts
        description: If true, the podcast will include posts from students as well
      - in: query
        name: position_after
        description: By default, discussions are sorted chronologically by creation
          date, youncan pass the id of another topic to have this one show up after
          the othernwhen they are listed
      - in: query
        name: published
        description: Whether this topic is published (true) or draft state (false)
      - in: query
        name: require_initial_post
        description: If true then a user may not respond to other replies until that
          user hasnmade an initial reply
      - in: query
        name: sort_by_rating
        description: If true, entries will be sorted by rating
      - in: query
        name: title
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
  /groups/{group_id}/discussion_topics/topic_id/entries:
    get:
      summary: List topic entries
      description: List topic entries.
      operationId: list-topic-entries
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identries-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
    post:
      summary: Post an entry
      description: Post an entry.
      operationId: post-an-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identries-post
      parameters:
      - in: query
        name: attachment
        description: a multipart/form-data form-field-style attachment
      - in: query
        name: message
        description: The body of the entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/rating:
    post:
      summary: Rate entry
      description: Rate entry.
      operationId: rate-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post
      parameters:
      - in: query
        name: rating
        description: A rating to set on this entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Rating
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read:
    delete:
      summary: Mark entry as unread
      description: Mark entry as unread.
      operationId: mark-entry-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Read
    put:
      summary: Mark entry as read
      description: Mark entry as read.
      operationId: mark-entry-as-read
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies:
    get:
      summary: List entry replies
      description: List entry replies.
      operationId: list-entry-replies
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Replies
    post:
      summary: Post a reply
      description: Post a reply.
      operationId: post-a-reply
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post
      parameters:
      - in: query
        name: attachment
        description: a multipart/form-data form-field-style attachment
      - in: query
        name: message
        description: The body of the entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Replies
  /groups/{group_id}/discussion_topics/topic_id/entries/{id}:
    delete:
      summary: Delete an entry
      description: Delete an entry.
      operationId: delete-an-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Id
    put:
      summary: Update an entry
      description: Update an entry.
      operationId: update-an-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesid-put
      parameters:
      - in: query
        name: message
        description: The updated body of the entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Id
  /groups/{group_id}/discussion_topics/topic_id/entry_list:
    get:
      summary: List entries
      description: List entries.
      operationId: list-entries
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identry-list-get
      parameters:
      - in: query
        name: ids[]
        description: A list of entry ids to retrieve
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entry
      - List
  /groups/{group_id}/discussion_topics/topic_id/read:
    delete:
      summary: Mark topic as unread
      description: Mark topic as unread.
      operationId: mark-topic-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
    put:
      summary: Mark topic as read
      description: Mark topic as read.
      operationId: mark-topic-as-read
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/read_all:
    delete:
      summary: Mark all entries as unread
      description: Mark all entries as unread.
      operationId: mark-all-entries-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-all-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
    put:
      summary: Mark all entries as read
      description: Mark all entries as read.
      operationId: mark-all-entries-as-read
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-all-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/subscribed:
    delete:
      summary: Unsubscribe from a topic
      description: Unsubscribe from a topic.
      operationId: unsubscribe-from-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
    put:
      summary: Subscribe to a topic
      description: Subscribe to a topic.
      operationId: subscribe-to-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
  /groups/{group_id}/discussion_topics/topic_id/view:
    get:
      summary: Get the full topic
      description: Get the full topic.
      operationId: get-the-full-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idview-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - View
  /groups/{group_id}/external_feeds:
    get:
      summary: List external feeds
      description: List external feeds.
      operationId: list-external-feeds
      x-api-path-slug: groupsgroup-idexternal-feeds-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
    post:
      summary: Create an external feed
      description: Create an external feed.
      operationId: create-an-external-feed
      x-api-path-slug: groupsgroup-idexternal-feeds-post
      parameters:
      - in: query
        name: header_match
        description: If given, only feed entries that contain this string in their
          title will benimported
      - in: query
        name: url
        description: The url to the external rss or atom feed
      - in: query
        name: verbosity
        description: 'Defaults to u201cfullu201dnn        n        n          Allowed
          values: full, truncate, link_only'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
  /groups/{group_id}/external_feeds/external_feed_id:
    delete:
      summary: Delete an external feed
      description: Delete an external feed.
      operationId: delete-an-external-feed
      x-api-path-slug: groupsgroup-idexternal-feedsexternal-feed-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
      - External
      - Feed
      - Id
  /groups/{group_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: groupsgroup-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: groupsgroup-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
  /groups/{group_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: groupsgroup-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Id
  /groups/{group_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: groupsgroup-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Quota
  /groups/{group_id}/folders:
    get:
      summary: List all folders
      description: List all folders.
      operationId: list-all-folders
      x-api-path-slug: groupsgroup-idfolders-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
    post:
      summary: Create folder
      description: Create folder.
      operationId: create-folder
      x-api-path-slug: groupsgroup-idfolders-post
      parameters:
      - in: query
        name: hidden
        description: Flag the folder as hidden
      - in: query
        name: locked
        description: Flag the folder as locked
      - in: query
        name: lock_at
        description: The datetime to lock the folder at
      - in: query
        name: name
        description: The name of the folder
      - in: query
        name: parent_folder_id
        description: The id of the folder to store the file in
      - in: query
        name: parent_folder_path
        description: The path of the folder to store the new folder in
      - in: query
        name: position
        description: Set an explicit sort position for the folder
      - in: query
        name: unlock_at
        description: The datetime to unlock the folder at
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
  /groups/{group_id}/folders/by_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: groupsgroup-idfoldersby-path-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - By
      - Path
  /groups/{group_id}/folders/by_path/*full_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: groupsgroup-idfoldersby-pathfull-path-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - By
      - Path
      - '*full'
      - Path
  /groups/{group_id}/folders/id:
    get:
      summary: Get folder
      description: Get folder.
      operationId: get-folder
      x-api-path-slug: groupsgroup-idfoldersid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - Id
  /groups/{group_id}/front_page:
    get:
      summary: Show front page
      description: Show front page.
      operationId: show-front-page
      x-api-path-slug: groupsgroup-idfront-page-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Front
      - Page
    put:
      summary: Update/create front page
      description: Update/create front page.
      operationId: updatecreate-front-page
      x-api-path-slug: groupsgroup-idfront-page-put
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Front
      - Page
  /groups/{group_id}/invite:
    post:
      summary: Invite others to a group
      description: Invite others to a group.
      operationId: invite-others-to-a-group
      x-api-path-slug: groupsgroup-idinvite-post
      parameters:
      - in: query
        name: invitees[]
        description: An array of email addresses to be sent invitations
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Invite
  /groups/{group_id}/memberships:
    get:
      summary: List group memberships
      description: List group memberships.
      operationId: list-group-memberships
      x-api-path-slug: groupsgroup-idmemberships-get
      parameters:
      - in: query
        name: filter_states[]
        description: Only list memberships with the given workflow_states
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
    post:
      summary: Create a membership
      description: Create a membership.
      operationId: create-a-membership
      x-api-path-slug: groupsgroup-idmemberships-post
      parameters:
      - in: query
        name: user_id
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
  /groups/{group_id}/memberships/membership_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
  /groups/{group_id}/pages:
    get:
      summary: List pages
      description: List pages.
      operationId: list-pages
      x-api-path-slug: groupsgroup-idpages-get
      parameters:
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: published
        description: If true, include only published paqes
      - in: query
        name: search_term
        description: The partial title of the pages to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
    post:
      summary: Create page
      description: Create page.
      operationId: create-page
      x-api-path-slug: groupsgroup-idpages-post
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[front_page]
        description: Set an unhidden page as the front page (if true)
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
  /groups/{group_id}/pages/url:
    delete:
      summary: Delete page
      description: Delete page.
      operationId: delete-page
      x-api-path-slug: groupsgroup-idpagesurl-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
    get:
      summary: Show page
      description: Show page.
      operationId: show-page
      x-api-path-slug: groupsgroup-idpagesurl-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
    put:
      summary: Update/create page
      description: Update/create page.
      operationId: updatecreate-page
      x-api-path-slug: groupsgroup-idpagesurl-put
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[front_page]
        description: Set an unhidden page as the front page (if true)
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
  /groups/{group_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: groupsgroup-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
  /groups/{group_id}/pages/url/revisions/latest:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionslatest-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Latest
  /groups/{group_id}/pages/url/revisions/{revision_id}:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
    post:
      summary: Revert to revision
      description: Revert to revision.
      operationId: revert-to-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-post
      parameters:
      - in: query
        name: revision_id
        description: The revision to revert to (use the List Revisions API to see
          available revisions)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
  /groups/{group_id}/preview_html:
    post:
      summary: Preview processed html
      description: Preview processed html.
      operationId: preview-processed-html
      x-api-path-slug: groupsgroup-idpreview-html-post
      parameters:
      - in: query
        name: html
        description: The html content to process
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Preview
      - Html
  /groups/{group_id}/tabs:
    get:
      summary: List available tabs for a course or group
      description: List available tabs for a course or group.
      operationId: list-available-tabs-for-a-course-or-group
      x-api-path-slug: groupsgroup-idtabs-get
      parameters:
      - in: query
        name: include[]
        description: 'Optionally include external tool tabs in the returned list of
          tabs (Onlynhas effect for courses, not groups)nn        n        n          Allowed
          values: external'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Tabs
  /groups/{group_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
  /groups/{group_id}/users:
    get:
      summary: List groups users
      description: List groups users.
      operationId: list-groups-users
      x-api-path-slug: groupsgroup-idusers-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cavatar_urlu201d: Include users&#39; avatar_urls'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
  /groups/{group_id}/users/user_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idusersuser-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idusersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idusersuser-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
  /group_categories/{group_category_id}/groups:
    get:
      summary: List groups in group category
      description: List groups in group category.
      operationId: list-groups-in-group-category
      x-api-path-slug: group-categoriesgroup-category-idgroups-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Groups
    post:
      summary: Create a group
      description: Create a group.
      operationId: create-a-group
      x-api-path-slug: group-categoriesgroup-category-idgroups-post
      parameters:
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Groups
  /group_categories/{group_category_id}:
    delete:
      summary: Delete a Group Category
      description: Delete a group category.
      operationId: delete-a-group-category
      x-api-path-slug: group-categoriesgroup-category-id-delete
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
    get:
      summary: Get a single group category
      description: Get a single group category.
      operationId: get-a-single-group-category
      x-api-path-slug: group-categoriesgroup-category-id-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
    put:
      summary: Update a Group Category
      description: Update a group category.
      operationId: update-a-group-category
      x-api-path-slug: group-categoriesgroup-category-id-put
      parameters:
      - in: query
        name: auto_leader
        description: 'Assigns group leaders automatically when generating and allocating
          studentsnto groups Valid values are:nu201cfirstu201dnnthe first student
          to be allocated to a group is the leadernu201crandomu201dnna random student
          from all members is chosen as the leadernnn        n        n          Allowed
          values: first, random'
      - in: query
        name: create_group_count
        description: Create this number of groups (Course Only)
      - in: query
        name: group_limit
        description: Limit the maximum number of users in each group (Course Only)
      - in: query
        name: name
        description: Name of the group category
      - in: query
        name: self_signup
        description: Allow students to sign up for a group themselves (Course Only)
      - in: query
        name: split_group_count
        description: (Deprecated) Create this number of groups, and evenly distribute
          studentsnamong them
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
  /group_categories/{group_category_id}/assign_unassigned_members:
    post:
      summary: Assign unassigned members
      description: Assign unassigned members.
      operationId: assign-unassigned-members
      x-api-path-slug: group-categoriesgroup-category-idassign-unassigned-members-post
      parameters:
      - in: query
        name: sync
        description: The assigning is done asynchronously by default
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Assign
      - Unassigned
      - Members
  /group_categories/{group_category_id}/users:
    get:
      summary: List users in group category
      description: List users in group category.
      operationId: list-users-in-group-category
      x-api-path-slug: group-categoriesgroup-category-idusers-get
      parameters:
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: unassigned
        description: Set this value to true if you wish only to search unassigned
          users in thengroup category
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Users
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
  /users/self/favorites/groups/{id}:
    delete:
      summary: Remove group from favorites
      description: Remove group from favorites.
      operationId: remove-group-from-favorites
      x-api-path-slug: usersselffavoritesgroupsid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the group to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
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