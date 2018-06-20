---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Member Get
  description: Retrieve a single member
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/groups:
    get:
      summary: Groups
      description: Fetch information about Meetup Groups.
      operationId: groups
      x-api-path-slug: 2groups-get
      parameters:
      - in: query
        name: category_id
        description: Only return groups in the specified category
        type: string
      - in: query
        name: country, city, state
        description: A valid country code, city and for the US, State
        type: string
      - in: query
        name: domain
        description: one or more custom group domains, separated by commas
        type: string
      - in: query
        name: fields
        description: optional result fields, separated by commas
        type: string
      - in: query
        name: group_id
        description: one or more separated by commas
        type: string
      - in: query
        name: group_urlname
        description: one or more separated by commas, includes no slashes
        type: string
      - in: query
        name: lat,lon
        description: A valid latitude and longitude, limits the returned groups to
          those within radius miles
        type: string
      - in: query
        name: member_id
        description: one or more separated by commas, for groups this member belongs
          to
        type: string
      - in: query
        name: organizer_id
        description: one or more organizer IDs, separated by commas
        type: string
      - in: query
        name: radius
        description: Radius, in miles for geographic requests, default 25 -- maximum
          100
        type: string
      - in: query
        name: topic
        description: Only return groups in the specified topic [one topic allowed]
        type: string
      - in: query
        name: topic, groupnum
        description: Return the group with this topic and number
        type: string
      - in: query
        name: zip
        description: A valid US zip code, limits the returned groups to those within
          radius miles
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /members:
    get:
      summary: Members
      description: API method for accessing members of Meetup Groups
      operationId: deprecated
      x-api-path-slug: members-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_id
        description: Return members in groups with these ID numbers, separated by
          commas
        type: string
      - in: query
        name: group_urlname
        description: Return members for the group with the given custom URL path
        type: string
      - in: query
        name: member_id
        description: Return the member with this ID
        type: string
      - in: query
        name: relation
        description: Supply the string self as the value for this parameter to get
          the information of the member linked to the API key making the request
        type: string
      - in: query
        name: service
        description: Match users by the external services theyve linked to their member
          account, specified as servicename:identifier
        type: string
      - in: query
        name: topic,groupnum
        description: Return members for the group with given topic and number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Members
  /2/members:
    get:
      summary: Members
      description: API method for accessing members of Meetup Groups
      operationId: members
      x-api-path-slug: 2members-get
      parameters:
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: group_id
        description: Return members in groups with these ID numbers, separated by
          commas
        type: string
      - in: query
        name: group_urlname
        description: Return members for the group with the given custom URL path
        type: string
      - in: query
        name: member_id
        description: Return the member with this ID
        type: string
      - in: query
        name: service
        description: Match users by the external services theyve linked to their member
          account, specified as servicename:identifier
        type: string
      - in: query
        name: topic,groupnum
        description: Return members for the group with given topic and number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/member/:id:
    get:
      summary: Member Get
      description: Retrieve a single member
      operationId: members
      x-api-path-slug: 2memberid-get
      parameters:
      - in: query
        name: fields
        description: comma-separate list of optional fields
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
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