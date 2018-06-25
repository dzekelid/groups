---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Appointment Groups API List appointment groups
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List appointment groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups
  tags: Appointment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groups-get-openapi.md
- name: Instructure Canvas Appointment Groups API Create an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Create an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups
  tags: Appointment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groups-post-openapi.md
- name: Instructure Canvas Appointment Groups API Delete an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Delete an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-delete-openapi.md
- name: Instructure Canvas Appointment Groups API Get a single appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Get a single appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-get-openapi.md
- name: Instructure Canvas Appointment Groups API Update an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Update an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsid-put-openapi.md
- name: Instructure Canvas Appointment Groups API List student group participants
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List student group participants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}/groups
  tags: Appointment,Groups,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsidgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsidgroups-get-openapi.md
- name: Instructure Canvas Appointment Groups API List user participants
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List user participants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}/users
  tags: Appointment,Groups,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/appointment-groupsidusers-get-openapi.md
- name: Instructure Canvas Appointment Groups API
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/openapi.md
- name: Instructure Canvas Courses API List assignment groups
  x-api-slug: instructure-canvas-courses-api
  description: List assignment groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups
  tags: Courses,Course,Id,Assignment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groups-get-openapi.md
- name: Instructure Canvas Courses API Create an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups
  tags: Courses,Course,Id,Assignment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groups-post-openapi.md
- name: Instructure Canvas Courses API Destroy an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Destroy an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-delete-openapi.md
- name: Instructure Canvas Courses API Get an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Get an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-get-openapi.md
- name: Instructure Canvas Courses API Edit an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Edit an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-put-openapi.md
- name: Instructure Canvas Courses API List the groups available in a context.
  x-api-slug: instructure-canvas-courses-api
  description: List the groups available in a context..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/groups
  tags: Courses,Course,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idgroups-get-openapi.md
- name: Instructure Canvas Courses API Get all outcome groups for context
  x-api-slug: instructure-canvas-courses-api
  description: Get all outcome groups for context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups
  tags: Courses,Course,Id,Outcome,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groups-get-openapi.md
- name: Instructure Canvas Courses API Delete an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Delete an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-delete-openapi.md
- name: Instructure Canvas Courses API Show an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Show an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-get-openapi.md
- name: Instructure Canvas Courses API Update an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Update an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsid-put-openapi.md
- name: Instructure Canvas Courses API Import an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Import an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/import
  tags: Courses,Course,Id,Outcome,Groups,Id,Import
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidimport-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidimport-post-openapi.md
- name: Instructure Canvas Courses API List linked outcomes
  x-api-slug: instructure-canvas-courses-api
  description: List linked outcomes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-get-openapi.md
- name: Instructure Canvas Courses API Create/link an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-post-openapi.md
- name: Instructure Canvas Courses API Unlink an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Unlink an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete-openapi.md
- name: Instructure Canvas Courses API Create/link an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-put-openapi.md
- name: Instructure Canvas Courses API List subgroups
  x-api-slug: instructure-canvas-courses-api
  description: List subgroups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/subgroups
  tags: Courses,Course,Id,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-get-openapi.md
- name: Instructure Canvas Courses API Create a subgroup
  x-api-slug: instructure-canvas-courses-api
  description: Create a subgroup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/subgroups
  tags: Courses,Course,Id,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-post-openapi.md
- name: Instructure Canvas Courses API Create a question group
  x-api-slug: instructure-canvas-courses-api
  description: Create a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroups-post-openapi.md
- name: Instructure Canvas Courses API Delete a question group
  x-api-slug: instructure-canvas-courses-api
  description: Delete a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single quiz group
  x-api-slug: instructure-canvas-courses-api
  description: Get a single quiz group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-get-openapi.md
- name: Instructure Canvas Courses API Update a question group
  x-api-slug: instructure-canvas-courses-api
  description: Update a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-put-openapi.md
- name: Instructure Canvas Courses API Reorder question groups
  x-api-slug: instructure-canvas-courses-api
  description: Reorder question groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}/reorder
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsidreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsidreorder-post-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/openapi.md
- name: Instructure Canvas Global API Delete an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Delete an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-delete-openapi.md
- name: Instructure Canvas Global API Show an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Show an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-get-openapi.md
- name: Instructure Canvas Global API Update an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Update an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsid-put-openapi.md
- name: Instructure Canvas Global API Import an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Import an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/import
  tags: Global,Outcome,Groups,Id,Import
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidimport-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidimport-post-openapi.md
- name: Instructure Canvas Global API List linked outcomes
  x-api-slug: instructure-canvas-global-api
  description: List linked outcomes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes
  tags: Global,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomes-get-openapi.md
- name: Instructure Canvas Global API Create/link an outcome
  x-api-slug: instructure-canvas-global-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes
  tags: Global,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomes-post-openapi.md
- name: Instructure Canvas Global API Unlink an outcome
  x-api-slug: instructure-canvas-global-api
  description: Unlink an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes/outcome_id
  tags: Global,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-delete-openapi.md
- name: Instructure Canvas Global API Create/link an outcome
  x-api-slug: instructure-canvas-global-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes/outcome_id
  tags: Global,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-put-openapi.md
- name: Instructure Canvas Global API List subgroups
  x-api-slug: instructure-canvas-global-api
  description: List subgroups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/subgroups
  tags: Global,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidsubgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidsubgroups-get-openapi.md
- name: Instructure Canvas Global API Create a subgroup
  x-api-slug: instructure-canvas-global-api
  description: Create a subgroup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/subgroups
  tags: Global,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidsubgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/globaloutcome-groupsidsubgroups-post-openapi.md
- name: Instructure Canvas Global API
  x-api-slug: instructure-canvas-global-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/openapi.md
- name: Instructure Canvas Groups API Create a group
  x-api-slug: instructure-canvas-groups-api
  description: Create a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groups-post-openapi.md
- name: Instructure Canvas Groups API Delete a group
  x-api-slug: instructure-canvas-groups-api
  description: Delete a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-get-openapi.md
- name: Instructure Canvas Groups API Edit a group
  x-api-slug: instructure-canvas-groups-api
  description: Edit a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-id-put-openapi.md
- name: Instructure Canvas Groups API Group activity stream
  x-api-slug: instructure-canvas-groups-api
  description: Group activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/activity_stream
  tags: Groups,Group,Id,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idactivity-stream-get-openapi.md
- name: Instructure Canvas Groups API Group activity stream summary
  x-api-slug: instructure-canvas-groups-api
  description: Group activity stream summary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/activity_stream/summary
  tags: Groups,Group,Id,Activity,Stream,Summary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idactivity-streamsummary-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idactivity-streamsummary-get-openapi.md
- name: Instructure Canvas Groups API Redirect to the assignment override for a group
  x-api-slug: instructure-canvas-groups-api
  description: Redirect to the assignment override for a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/assignments/assignment_id/override
  tags: Groups,Group,Id,Assignments,Assignment,Id,Override
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-openapi.md
- name: Instructure Canvas Groups API List conferences
  x-api-slug: instructure-canvas-groups-api
  description: List conferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/conferences
  tags: Groups,Group,Id,Conferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idconferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idconferences-get-openapi.md
- name: Instructure Canvas Groups API List content exports
  x-api-slug: instructure-canvas-groups-api
  description: List content exports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports
  tags: Groups,Group,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exports-get-openapi.md
- name: Instructure Canvas Groups API Export content
  x-api-slug: instructure-canvas-groups-api
  description: Export content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports
  tags: Groups,Group,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exports-post-openapi.md
- name: Instructure Canvas Groups API Show content export
  x-api-slug: instructure-canvas-groups-api
  description: Show content export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports/id
  tags: Groups,Group,Id,Content,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-exportsid-get-openapi.md
- name: Instructure Canvas Groups API List licenses
  x-api-slug: instructure-canvas-groups-api
  description: List licenses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_licenses
  tags: Groups,Group,Id,Content,Licenses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-licenses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-licenses-get-openapi.md
- name: Instructure Canvas Groups API List content migrations
  x-api-slug: instructure-canvas-groups-api
  description: List content migrations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations
  tags: Groups,Group,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrations-get-openapi.md
- name: Instructure Canvas Groups API Create a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Create a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations
  tags: Groups,Group,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrations-post-openapi.md
- name: Instructure Canvas Groups API List migration issues
  x-api-slug: instructure-canvas-groups-api
  description: List migration issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get-openapi.md
- name: Instructure Canvas Groups API Get a migration issue
  x-api-slug: instructure-canvas-groups-api
  description: Get a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get-openapi.md
- name: Instructure Canvas Groups API Update a migration issue
  x-api-slug: instructure-canvas-groups-api
  description: Update a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put-openapi.md
- name: Instructure Canvas Groups API Get a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Get a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/id
  tags: Groups,Group,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsid-get-openapi.md
- name: Instructure Canvas Groups API Update a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Update a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/id
  tags: Groups,Group,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsid-put-openapi.md
- name: Instructure Canvas Groups API List Migration Systems
  x-api-slug: instructure-canvas-groups-api
  description: List migration systems.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/migrators
  tags: Groups,Group,Id,Content,Migrations,Migrators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsmigrators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idcontent-migrationsmigrators-get-openapi.md
- name: Instructure Canvas Groups API List discussion topics
  x-api-slug: instructure-canvas-groups-api
  description: List discussion topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics
  tags: Groups,Group,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topics-get-openapi.md
- name: Instructure Canvas Groups API Create a new discussion topic
  x-api-slug: instructure-canvas-groups-api
  description: Create a new discussion topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics
  tags: Groups,Group,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topics-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topics-post-openapi.md
- name: Instructure Canvas Groups API Reorder pinned topics
  x-api-slug: instructure-canvas-groups-api
  description: Reorder pinned topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/reorder
  tags: Groups,Group,Id,Discussion,Topics,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicsreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicsreorder-post-openapi.md
- name: Instructure Canvas Groups API Delete a topic
  x-api-slug: instructure-canvas-groups-api
  description: Delete a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single topic
  x-api-slug: instructure-canvas-groups-api
  description: Get a single topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-get-openapi.md
- name: Instructure Canvas Groups API Update a topic
  x-api-slug: instructure-canvas-groups-api
  description: Update a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-put-openapi.md
- name: Instructure Canvas Groups API List topic entries
  x-api-slug: instructure-canvas-groups-api
  description: List topic entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-get-openapi.md
- name: Instructure Canvas Groups API Post an entry
  x-api-slug: instructure-canvas-groups-api
  description: Post an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-post-openapi.md
- name: Instructure Canvas Groups API Rate entry
  x-api-slug: instructure-canvas-groups-api
  description: Rate entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/rating
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Rating
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post-openapi.md
- name: Instructure Canvas Groups API Mark entry as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark entry as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete-openapi.md
- name: Instructure Canvas Groups API Mark entry as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark entry as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put-openapi.md
- name: Instructure Canvas Groups API List entry replies
  x-api-slug: instructure-canvas-groups-api
  description: List entry replies.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get-openapi.md
- name: Instructure Canvas Groups API Post a reply
  x-api-slug: instructure-canvas-groups-api
  description: Post a reply.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post-openapi.md
- name: Instructure Canvas Groups API Delete an entry
  x-api-slug: instructure-canvas-groups-api
  description: Delete an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{id}
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-delete-openapi.md
- name: Instructure Canvas Groups API Update an entry
  x-api-slug: instructure-canvas-groups-api
  description: Update an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{id}
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-put-openapi.md
- name: Instructure Canvas Groups API List entries
  x-api-slug: instructure-canvas-groups-api
  description: List entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entry_list
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entry,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identry-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identry-list-get-openapi.md
- name: Instructure Canvas Groups API Mark topic as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark topic as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-delete-openapi.md
- name: Instructure Canvas Groups API Mark topic as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark topic as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-put-openapi.md
- name: Instructure Canvas Groups API Mark all entries as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark all entries as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read_all
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-delete-openapi.md
- name: Instructure Canvas Groups API Mark all entries as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark all entries as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read_all
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-put-openapi.md
- name: Instructure Canvas Groups API Unsubscribe from a topic
  x-api-slug: instructure-canvas-groups-api
  description: Unsubscribe from a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/subscribed
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-delete-openapi.md
- name: Instructure Canvas Groups API Subscribe to a topic
  x-api-slug: instructure-canvas-groups-api
  description: Subscribe to a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/subscribed
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-put-openapi.md
- name: Instructure Canvas Groups API Get the full topic
  x-api-slug: instructure-canvas-groups-api
  description: Get the full topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/view
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,View
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idview-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idview-get-openapi.md
- name: Instructure Canvas Groups API List external feeds
  x-api-slug: instructure-canvas-groups-api
  description: List external feeds.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds
  tags: Groups,Group,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feeds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feeds-get-openapi.md
- name: Instructure Canvas Groups API Create an external feed
  x-api-slug: instructure-canvas-groups-api
  description: Create an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds
  tags: Groups,Group,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feeds-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feeds-post-openapi.md
- name: Instructure Canvas Groups API Delete an external feed
  x-api-slug: instructure-canvas-groups-api
  description: Delete an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds/external_feed_id
  tags: Groups,Group,Id,External,Feeds,External,Feed,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feedsexternal-feed-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idexternal-feedsexternal-feed-id-delete-openapi.md
- name: Instructure Canvas Groups API List files
  x-api-slug: instructure-canvas-groups-api
  description: List files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files
  tags: Groups,Group,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfiles-get-openapi.md
- name: Instructure Canvas Groups API Upload a file
  x-api-slug: instructure-canvas-groups-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files
  tags: Groups,Group,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfiles-post-openapi.md
- name: Instructure Canvas Groups API Get file
  x-api-slug: instructure-canvas-groups-api
  description: Get file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files/id
  tags: Groups,Group,Id,Files,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfilesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfilesid-get-openapi.md
- name: Instructure Canvas Groups API Get quota information
  x-api-slug: instructure-canvas-groups-api
  description: Get quota information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files/quota
  tags: Groups,Group,Id,Files,Quota
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfilesquota-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfilesquota-get-openapi.md
- name: Instructure Canvas Groups API List all folders
  x-api-slug: instructure-canvas-groups-api
  description: List all folders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders
  tags: Groups,Group,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfolders-get-openapi.md
- name: Instructure Canvas Groups API Create folder
  x-api-slug: instructure-canvas-groups-api
  description: Create folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders
  tags: Groups,Group,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfolders-post-openapi.md
- name: Instructure Canvas Groups API Resolve path
  x-api-slug: instructure-canvas-groups-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/by_path
  tags: Groups,Group,Id,Folders,By,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersby-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersby-path-get-openapi.md
- name: Instructure Canvas Groups API Resolve path
  x-api-slug: instructure-canvas-groups-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/by_path/*full_path
  tags: Groups,Group,Id,Folders,By,Path,*full,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersby-pathfull-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersby-pathfull-path-get-openapi.md
- name: Instructure Canvas Groups API Get folder
  x-api-slug: instructure-canvas-groups-api
  description: Get folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/id
  tags: Groups,Group,Id,Folders,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfoldersid-get-openapi.md
- name: Instructure Canvas Groups API Show front page
  x-api-slug: instructure-canvas-groups-api
  description: Show front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/front_page
  tags: Groups,Group,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfront-page-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfront-page-get-openapi.md
- name: Instructure Canvas Groups API Update/create front page
  x-api-slug: instructure-canvas-groups-api
  description: Update/create front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/front_page
  tags: Groups,Group,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfront-page-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idfront-page-put-openapi.md
- name: Instructure Canvas Groups API Invite others to a group
  x-api-slug: instructure-canvas-groups-api
  description: Invite others to a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/invite
  tags: Groups,Group,Id,Invite
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idinvite-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idinvite-post-openapi.md
- name: Instructure Canvas Groups API List group memberships
  x-api-slug: instructure-canvas-groups-api
  description: List group memberships.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmemberships-get-openapi.md
- name: Instructure Canvas Groups API Create a membership
  x-api-slug: instructure-canvas-groups-api
  description: Create a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmemberships-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmemberships-post-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-openapi.md
- name: Instructure Canvas Groups API List pages
  x-api-slug: instructure-canvas-groups-api
  description: List pages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages
  tags: Groups,Group,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpages-get-openapi.md
- name: Instructure Canvas Groups API Create page
  x-api-slug: instructure-canvas-groups-api
  description: Create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages
  tags: Groups,Group,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpages-post-openapi.md
- name: Instructure Canvas Groups API Delete page
  x-api-slug: instructure-canvas-groups-api
  description: Delete page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-delete-openapi.md
- name: Instructure Canvas Groups API Show page
  x-api-slug: instructure-canvas-groups-api
  description: Show page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-get-openapi.md
- name: Instructure Canvas Groups API Update/create page
  x-api-slug: instructure-canvas-groups-api
  description: Update/create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurl-put-openapi.md
- name: Instructure Canvas Groups API List revisions
  x-api-slug: instructure-canvas-groups-api
  description: List revisions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions
  tags: Groups,Group,Id,Pages,Url,Revisions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisions-get-openapi.md
- name: Instructure Canvas Groups API Show revision
  x-api-slug: instructure-canvas-groups-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/latest
  tags: Groups,Group,Id,Pages,Url,Revisions,Latest
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionslatest-get-openapi.md
- name: Instructure Canvas Groups API Show revision
  x-api-slug: instructure-canvas-groups-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/{revision_id}
  tags: Groups,Group,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-get-openapi.md
- name: Instructure Canvas Groups API Revert to revision
  x-api-slug: instructure-canvas-groups-api
  description: Revert to revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/{revision_id}
  tags: Groups,Group,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-post-openapi.md
- name: Instructure Canvas Groups API Preview processed html
  x-api-slug: instructure-canvas-groups-api
  description: Preview processed html.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/preview_html
  tags: Groups,Group,Id,Preview,Html
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpreview-html-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idpreview-html-post-openapi.md
- name: Instructure Canvas Groups API List available tabs for a course or group
  x-api-slug: instructure-canvas-groups-api
  description: List available tabs for a course or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/tabs
  tags: Groups,Group,Id,Tabs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idtabs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idtabs-get-openapi.md
- name: Instructure Canvas Groups API Remove usage rights
  x-api-slug: instructure-canvas-groups-api
  description: Remove usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/usage_rights
  tags: Groups,Group,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusage-rights-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusage-rights-delete-openapi.md
- name: Instructure Canvas Groups API Set usage rights
  x-api-slug: instructure-canvas-groups-api
  description: Set usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/usage_rights
  tags: Groups,Group,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusage-rights-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusage-rights-put-openapi.md
- name: Instructure Canvas Groups API List groups users
  x-api-slug: instructure-canvas-groups-api
  description: List groups users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users
  tags: Groups,Group,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusers-get-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/groupsgroup-idusersuser-id-put-openapi.md
- name: Instructure Canvas Groups API List groups in group category
  x-api-slug: instructure-canvas-groups-api
  description: List groups in group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/groups
  tags: Group,Categories,Group,Category,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/group-categoriesgroup-category-idgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/group-categoriesgroup-category-idgroups-get-openapi.md
- name: Instructure Canvas Groups API Create a group
  x-api-slug: instructure-canvas-groups-api
  description: Create a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/groups
  tags: Group,Categories,Group,Category,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/group-categoriesgroup-category-idgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/group-categoriesgroup-category-idgroups-post-openapi.md
- name: Instructure Canvas Groups API
  x-api-slug: instructure-canvas-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/openapi.md
- name: Instructure Canvas Users API Reset group favorites
  x-api-slug: instructure-canvas-users-api
  description: Reset group favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroups-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroups-delete-openapi.md
- name: Instructure Canvas Users API List favorite groups
  x-api-slug: instructure-canvas-users-api
  description: List favorite groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroups-get-openapi.md
- name: Instructure Canvas Users API Remove group from favorites
  x-api-slug: instructure-canvas-users-api
  description: Remove group from favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroupsid-delete-openapi.md
- name: Instructure Canvas Users API Add group to favorites
  x-api-slug: instructure-canvas-users-api
  description: Add group to favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroupsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselffavoritesgroupsid-post-openapi.md
- name: Instructure Canvas Users API List your groups
  x-api-slug: instructure-canvas-users-api
  description: List your groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/groups
  tags: Users,Self,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselfgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/usersselfgroups-get-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---