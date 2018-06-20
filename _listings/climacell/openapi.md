---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 1
info:
  title: ClimaCell API
  description: the-climacell-rest-api-provides-access-to-high-resolution-weather-data-for-locations-across-the-u-s--with-global-data-coming-soon--it-uses-https-and-requires-an-access-token-key--the-api-requests-carry-query-parameters-and-the-responses-return-results-in-json-format-
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: Get Groups
      description: |-
        ### List all Groups
        Page through a list of all your groups. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-groupspage-through-a-list-of-all-your-groups-you-can-specify-the-maximum-number-of-results
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
    post:
      summary: Post Groups
      description: |-
        ### Create a Group

        Creates a new Group, and name it. The system attaches a unique ID to each group you create. This ID is used to refer to the group and manage it in the following ```groups``` API calls.
      operationId: -create-a-groupcreates-a-new-group-and-name-it-the-system-attaches-a-unique-id-to-each-group-you-cre
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
  /groups/{group_id}:
    get:
      summary: Get Groups Group
      description: |-
        ### Retrieve a Group

        Get a single group with its information by specifying its ```group_id```.
      operationId: -retrieve-a-groupget-a-single-group-with-its-information-by-specifying-its-group-id
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
    put:
      summary: Put Groups Group
      description: |-
        ### Update a Group

        Updates the name of a Group with a ```group_id```.
      operationId: -update-a-groupupdates-the-name-of-a-group-with-a-group-id
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_id
        description: UUID of the Group
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
    delete:
      summary: Delete Groups Group
      description: |-
        ### Delete a Group

        Removes a Group with the ```group_id``` from the system. Note that the user information will be lost.
      operationId: -delete-a-groupremoves-a-group-with-the-group-id-from-the-system-note-that-the-user-information-will
      x-api-path-slug: groupsgroup-id-delete
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
  /groups/{group_id}/members:
    get:
      summary: Get Groups Group Members
      description: |-
        ### List all Group Members
        Page through a list of all members of a group with a ```group_id```. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-group-memberspage-through-a-list-of-all-members-of-a-group-with-a-group-id-you-can-specify
      x-api-path-slug: groupsgroup-idmembers-get
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
    post:
      summary: Post Groups Group Members
      description: "### Create a Group Member\n\nAdds a member to a group with a ```group_id```.
        \u200BMake sure you provide an accurate email address and/or phone number
        or alerts will not be received by the member."
      operationId: -create-a-group-memberadds-a-member-to-a-group-with-a-group-id-make-sure-you-provide-an-accurate-ema
      x-api-path-slug: groupsgroup-idmembers-post
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_id
        description: UUID of the Group
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
  /groups/{group_id}/members/{member_id}:
    put:
      summary: Put Groups Group Members Member
      description: |-
        ### Delete a Group Member
        Updates a member with the ```member_id``` to the group with a ```group_id```.
      operationId: -delete-a-group-memberupdates-a-member-with-the-member-id-to-the-group-with-a-group-id
      x-api-path-slug: groupsgroup-idmembersmember-id-put
      parameters:
      - in: body
        name: group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: group_id
        description: UUID of the Group
      - in: path
        name: member_id
        description: UUID of the User
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
      - Member
    delete:
      summary: Delete Groups Group Members Member
      description: |-
        ### Delete a Group Member
        Removes a member with the ```member_id``` from the group with a ```group_id```.
      operationId: -delete-a-group-memberremoves-a-member-with-the-member-id-from-the-group-with-a-group-id
      x-api-path-slug: groupsgroup-idmembersmember-id-delete
      parameters:
      - in: path
        name: group_id
        description: UUID of the Group
      - in: path
        name: member_id
        description: UUID of the User
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Groups
      - Group
      - Members
      - Member
---