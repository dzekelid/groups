---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToMeeting Historical meetings by group
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  version: 1.0.0
host: api.getgo.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: Groups
      description: List all groups for an account. This API call is only available
        to users with the admin role.
      operationId: GroupsGet
      x-api-path-slug: groups-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{groupKey}/upcomingMeetings:
    get:
      summary: Upcoming meetings by group
      description: Get upcoming meetings for a specified group. This API call is only
        available to users with the admin role. This API call can be used only for
        groups with maximum 50 organizers.
      operationId: GroupsUpcomingMeetingsByGroupKeyGet
      x-api-path-slug: groupsgroupkeyupcomingmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: groupKey
      responses:
        200:
          description: OK
      tags:
      - Upcoming
      - Meetings
      - By
      - Group
  /groups/{groupkey}/organizers:
    get:
      summary: Organizers by group
      description: Returns all the organizers within a specific group. This API call
        is only available to users with the admin role.
      operationId: GroupsOrganizersByGroupkeyGet
      x-api-path-slug: groupsgroupkeyorganizers-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: groupkey
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - By
      - Group
  /groups/{groupkey}/attendees:
    get:
      summary: Attendees by group
      description: Returns all attendees for all meetings within specified date range
        held by organizers within the specified group. This API call is only available
        to users with the admin role. This API call can be used only for groups with
        maximum 50 organizers.
      operationId: GroupsAttendeesByGroupkeyGet
      x-api-path-slug: groupsgroupkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: groupkey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - By
      - Group
  /groups/{groupKey}/organizers:
    post:
      summary: Organizer in group
      description: "Creates a new organizer and sends an email to the email address
        defined in request. This API call is only available to users with the admin
        role. You may also pass 'G2W' or 'G2T' or 'OPENVOICE' as productType variables,
        creating organizers for those products. A G2W or G2T organizer will also have
        access to G2M.\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"organizerEmail\"\t\t\t\"valid.org@email.com\"\t\t\tString
        with valid email syntax\t\t\r\n\t\t\"firstName\"\t\t\t\"First\"\t\t\tString
        - max 25 characters\t\t\r\n\t\t\"lastName\"\t\t\t\"Last\"\t\t\tString - max
        25 characters\t\t\r\n\t\t\"productType\"\t\t\t\"G2M\"\t\t\tMust be: G2M, G2W,
        G2T, OV"
      operationId: GroupsOrganizersByGroupKeyPost
      x-api-path-slug: groupsgroupkeyorganizers-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: groupKey
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - In
      - Group
  /groups/{groupkey}/historicalMeetings:
    get:
      summary: Historical meetings by group
      description: 'Get historical meetings for the specified group that started within
        the specified date/time range. This API call is only available to users with
        the admin role. This API call is restricted to groups with a maximum of 50
        organizers. Remark: Meetings which are still ongoing at the time of the request
        are NOT contained in the result array.'
      operationId: GroupsHistoricalMeetingsByGroupkeyGet
      x-api-path-slug: groupsgroupkeyhistoricalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: groupkey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
      - By
      - Group
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