---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Recommend Group Topics
  description: Recommends suggestions for group topics based on a text search or other
    topics
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
    post:
      summary: Member Edit
      description: Edit the authorized member's attributes
      operationId: members
      x-api-path-slug: 2memberid-post
      parameters:
      - in: query
        name: add_topics
        description: Comma-delimited list of topics ids to add to your alert list
        type: string
      - in: query
        name: bio
        description: Free form text passage about you
        type: string
      - in: query
        name: bio_privacy
        description: Controls the visibility of the members bio
        type: string
      - in: query
        name: birthday
        description: Day you were born
        type: string
      - in: query
        name: city
        description: City name for your location
        type: string
      - in: query
        name: city_id
        description: Valid city id from /2/cities method
        type: string
      - in: query
        name: country
        description: Valid country code for your location
        type: string
      - in: query
        name: facebook_privacy
        description: Controls the visibility of the members facebook connection
        type: string
      - in: query
        name: gender
        description: Your gender (used for better recommendations)
        type: string
      - in: query
        name: groups_privacy
        description: Controls the visibility of the members groups
        type: string
      - in: query
        name: hometown
        description: Hometown of member
        type: string
      - in: query
        name: lang
        description: Language preference used on the site
        type: string
      - in: query
        name: lat
        description: latitude of city
        type: string
      - in: query
        name: lon
        description: longitude of city
        type: string
      - in: query
        name: messaging_pref
        description: This specifies the members preference for being contacted from
          members on the site
        type: string
      - in: query
        name: name
        description: The name of the current member
        type: string
      - in: query
        name: photos_privacy
        description: Controls the visibility of the members photos
        type: string
      - in: query
        name: photo_id
        description: A valid photo_id from the members photos to set as the main profile
          photo
        type: string
      - in: query
        name: radius
        description: radius, in miles to search for city given a lat and lon
        type: string
      - in: query
        name: remove_topics
        description: Comma-delimited list of topic ids to remove from your alert list
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      - in: query
        name: topics_privacy
        description: Controls the visibility of the members topics
        type: string
      - in: query
        name: zip
        description: Valid zip code for city
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /2/event_ratings:
    get:
      summary: Ratings v2
      description: API method for accessing Meetup comments
      operationId: events
      x-api-path-slug: 2event-ratings-get
      parameters:
      - in: query
        name: event_id
        description: The ID of the event to fetch ratings data for
        type: string
      - in: query
        name: member_id
        description: The ID of a member to filter ratings on
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /2/group_photo:
    post:
      summary: Group Photo Upload
      description: Uploads a new Meetup Group photo. To change other Group settings
        use the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
      operationId: groups
      x-api-path-slug: 2group-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: group_id
        description: Group ID for the target group
        type: string
      - in: query
        name: group_urlname
        description: Group urlname
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the groups main photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /2/member_photo:
    post:
      summary: Member Photo Upload
      description: Uploads a photo to be associated with a Member
      operationId: members
      x-api-path-slug: 2member-photo-post
      parameters:
      - in: query
        name: await
        description: If true, this ensures a response will not be returned until the
          upload is accessible
        type: string
      - in: query
        name: main
        description: Set to true to have this photo become the members main profile
          photo
        type: string
      - in: query
        name: photo
        description: The photo, encoded as multipart/form-data
        type: string
      - in: query
        name: sync_matching_photo
        description: When set to true and main is set to true, this will replace all
          group profile photos matching the current photo with the provided replacement
        type: string
      - in: query
        name: sync_photo
        description: When set to true, this parameter will sync all of the group profile
          photos for the member with the provided photo_id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Member
  /groups:
    get:
      summary: Groups
      description: API method for accessing meetup groups
      operationId: deprecated
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: country, city, state
        description: A valid country code, city and for the US, State
        type: string
      - in: query
        name: fields
        description: Set to short_link to include shortened group URLs in response
          items
        type: string
      - in: query
        name: group_urlname
        description: Return the group with this custom url path (e
        type: string
      - in: query
        name: id
        description: Only return groups with the specified IDs [separate ID numbers
          with commas]
        type: string
      - in: query
        name: lat,lon
        description: A valid latitude and longitude, limits the returned groups to
          those within radius miles
        type: string
      - in: query
        name: member_id
        description: A member id number, limits results set to only those groups that
          the member specified by this id is currently a member of (excludes private
          groups, unless the member_id is the same as that of the member making the
          request)
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
        name: visibility
        description: Set to members or public to restrict to groups of a particular
          visibility
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
  /:urlname/abuse_reports:
    post:
      summary: Report Group
      description: Submits a new abuse report for a target group. Abuse reports will
        be followed up on by our Community Support team.
      operationId: abuse
      x-api-path-slug: urlnameabuse-reports-post
      parameters:
      - in: query
        name: type
        description: A required identifier for type of abuse you are reporting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /find/groups:
    get:
      summary: Find Groups
      description: Text, location, category and friend-based group searches
      operationId: groups
      x-api-path-slug: findgroups-get
      parameters:
      - in: query
        name: category
        description: Comma-delimited list of numeric category ids
        type: string
      - in: query
        name: country
        description: A valid two character country code, defaults to US
        type: string
      - in: query
        name: fallback_suggestions
        description: boolean indicator of whether or not to return a list of curated
          suggestions for groups if we cant find groups matching your criteria
        type: string
      - in: query
        name: fields
        description: Request that additional fields (separated by commas) be included
          in the output
        type: string
      - in: query
        name: filter
        description: Determines which groups are returned
        type: string
      - in: query
        name: lat
        description: Approximate latitude
        type: string
      - in: query
        name: location
        description: Raw text location query
        type: string
      - in: query
        name: lon
        description: Approximate longitude
        type: string
      - in: query
        name: radius
        description: Radius in miles
        type: string
      - in: query
        name: self_groups
        description: set to include or exclude Meetups the authorized member belongs
          to; default is include
        type: string
      - in: query
        name: text
        description: Raw full text search query
        type: string
      - in: query
        name: topic_id
        description: Comma-delimited list of numeric topic ids
        type: string
      - in: query
        name: upcoming_events
        description: If true, filters text and category based searches on groups that
          have upcoming events
        type: string
      - in: query
        name: zip
        description: Zipcode of location to limit search to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Groups
  /:urlname/members:
    get:
      summary: Group Profile list
      description: Get a list of Meetup group members
      operationId: profiles
      x-api-path-slug: urlnamemembers-get
      parameters:
      - in: query
        name: desc
        description: Boolean value controling sort order of results
        type: string
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: filter
        description: May be set to stepup_eligible to return only members eligible
          to step up as organizer
        type: string
      - in: query
        name: order
        description: Orders results according to definitions listed below
        type: string
      - in: query
        name: page
        description: Number of requested members to return
        type: string
      - in: query
        name: role
        description: May be set to leads to filter returned members on the lead team
        type: string
      - in: query
        name: status
        description: A comma-delimited list of member statuses
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    post:
      summary: Group Join
      description: This method allows an authenticated member to join a group by creating
        a profile
      operationId: profiles
      x-api-path-slug: urlnamemembers-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /find/:urlname/members:
    get:
      summary: Group Profile search
      description: |-
        Find group member profiles by name.
        Member's who very recently joined or left the group may not be immediately searchable
      operationId: profiles
      x-api-path-slug: findurlnamemembers-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: order
        description: Orders results according to definitions listed below
        type: string
      - in: query
        name: page
        description: Number of requested members to return
        type: string
      - in: query
        name: query
        description: The name to search for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
      - Search
  /:urlname:
    get:
      summary: Get Group
      description: Fetches a Meetup group by urlname
      operationId: groups
      x-api-path-slug: urlname-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    post:
      summary: Group Edit
      description: Allows organizers to edit their Meetup group information. To change
        group topics, see the [add](/meetup_api/docs/:urlname/topics/#add) and [remove](/meetup_api/docs/:urlname/topics/#remove)
        topics endpoints. To change group photo use the [Group photo upload](/meetup_api/docs/2/group_photo/#create)
        endpoint. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
        permission.
      operationId: groups
      x-api-path-slug: urlname-post
      parameters:
      - in: query
        name: add_topics
        description: Comma-delimited list of topic ids to associate with group
        type: string
      - in: query
        name: country
        description: The ISO_3166-1 country code for the country which contains the
          city
        type: string
      - in: query
        name: description
        description: Summary of what the Meetup group is about in simple HTML format
        type: string
      - in: query
        name: dryrun
        description: Boolean parameter that will cause this endpoint to apply all
          validation rules without actually saving changes in which case the response
          will only reflect the groups current attributes
        type: string
      - in: query
        name: ga_code
        description: Google Analytics code for group
        type: string
      - in: query
        name: join_mode
        description: Controls how members are let into the group
        type: string
      - in: query
        name: key_photo
        description: Groups primary photo
        type: string
      - in: query
        name: list_addr
        description: Mailing list prefix
        type: string
      - in: query
        name: list_mode
        description: Defines policy for who can post to the group mailing list
        type: string
      - in: query
        name: name
        description: Display name of the group
        type: string
      - in: query
        name: photo_req
        description: Indicates that a member must provide a photo before joining
        type: string
      - in: query
        name: questions_req
        description: Indicates that provided questions are required before joining
        type: string
      - in: query
        name: question_edit_{id}
        description: Edits a current profile question identified by an id in the parameter
          name
        type: string
      - in: query
        name: question_{index}
        description: A new profile question defined in the order of index provided
          in the request parameter name
        type: string
      - in: query
        name: remove_topics
        description: Comma-delimited list of topic ids to disassociate with group
        type: string
      - in: query
        name: urlname
        description: Name used for the groups web address on meetup
        type: string
      - in: query
        name: visibility
        description: Restricts group visibility for non-members
        type: string
      - in: query
        name: welcome_message
        description: Message sent to members after they join
        type: string
      - in: query
        name: who
        description: What members of the group will be called
        type: string
      - in: query
        name: zip
        description: The ZIP code of the city
        type: string
      - in: query
        name: '{service}_uri'
        description: A URI for a social network service
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /self/groups:
    get:
      summary: Member groups
      description: |-
        Lists the authenticated member's groups in the order of leadership,
        next upcoming event, then alphabetical order by name
      operationId: groups
      x-api-path-slug: selfgroups-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited list of optional fields to append to the response
        type: string
      - in: query
        name: page
        description: Number of groups to return in a single page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Members
      - Groups
  /pro/:urlname/groups:
    get:
      summary: Search Pro Groups
      description: Name and statistics range search for the meetup groups belonging
        to Pro organization.
      operationId: pro
      x-api-path-slug: prourlnamegroups-get
      parameters:
      - in: query
        name: active_within_days
        description: 'Positive Integer: including only those groups that had event
          in the last specified days'
        type: string
      - in: query
        name: average_age_max
        description: 'Positive Integer: Maximum range of the average age of the members'
        type: string
      - in: query
        name: average_age_min
        description: 'Positive Integer: Minumum range of the average age of the members'
        type: string
      - in: query
        name: category
        description: 'List of Integers: the ids of the category of the group'
        type: string
      - in: query
        name: chapters
        description: 'List of Integer: the chapter ids that may belong to the organization'
        type: string
      - in: query
        name: chapter_urlname
        description: 'List of String: the urlnames of chapters that may belong to
          the organization'
        type: string
      - in: query
        name: country
        description: 'String: Country'
        type: string
      - in: query
        name: desc
        description: 'List of Boolean: whether to sort ascending or decending on each
          attributes in `order`'
        type: string
      - in: query
        name: excluded_chapters
        description: 'List of Integer: the chapters to exclude from the result'
        type: string
      - in: query
        name: founded_date_max
        description: 'Milliseconds since epoch: Maximum range of the founded dates
          of the groups'
        type: string
      - in: query
        name: founded_date_min
        description: 'Milliseconds since epoch: Minumum range of the founded dates
          of the groups'
        type: string
      - in: query
        name: inactive_within_days
        description: 'Positive Integer: including only those groups that did not have
          event in the last specified days'
        type: string
      - in: query
        name: last_event_max
        description: 'Milliseconds since epoch: Maximum range of the date that the
          last meetup happened'
        type: string
      - in: query
        name: last_event_min
        description: 'Milliseconds since epoch: Minumum range of the date that the
          last meetup happened'
        type: string
      - in: query
        name: lat
        description: 'Float: Latitude'
        type: string
      - in: query
        name: location
        description: 'String: Raw location'
        type: string
      - in: query
        name: lon
        description: 'Float: Longitude'
        type: string
      - in: query
        name: member_count_max
        description: 'Positive Integer: Maximum range of the number of members'
        type: string
      - in: query
        name: member_count_min
        description: 'Positive Integer: Minimum range of the number of members'
        type: string
      - in: query
        name: name
        description: 'String: Name of the group looking for'
        type: string
      - in: query
        name: next_event_max
        description: 'Milliseconds since epoch: Maximum range of the date that the
          next meetup is scheduled'
        type: string
      - in: query
        name: next_event_min
        description: 'Milliseconds since epoch: Minumum range of the date that the
          next meetup is scheduled'
        type: string
      - in: query
        name: offset
        description: 'Positive Integer: the page offset'
        type: string
      - in: query
        name: order
        description: 'List of String: attributes to sort on'
        type: string
      - in: query
        name: page
        description: 'Positive Integer: the size of page window'
        type: string
      - in: query
        name: past_events_max
        description: 'Positive Integer: Maximum range of the number of the past events
          held'
        type: string
      - in: query
        name: past_events_min
        description: 'Positive Integer: Minumum range of the number of the past events
          held'
        type: string
      - in: query
        name: past_rsvps_max
        description: 'Positive Integer: Maximum range of the total number of past
          RSVPs'
        type: string
      - in: query
        name: past_rsvps_min
        description: 'Positive Integer: Minumum range of the total number of past
          RSVPs'
        type: string
      - in: query
        name: pro_join_date_max
        description: 'Milliseconds since epoch: Maximum range of the dates the groups
          joined Pro organization'
        type: string
      - in: query
        name: pro_join_date_min
        description: 'Milliseconds since epoch: Minumum range of the dates the groups
          joined Pro organization'
        type: string
      - in: query
        name: query
        description: 'String: raw query to search from group name, description, leadership
          member name, or city'
        type: string
      - in: query
        name: radius
        description: 'String: `global`, `smart`, or search radius in Float'
        type: string
      - in: query
        name: repeat_rsvpers_max
        description: 'Positive Integer: Maximum range of the average number of repeat
          rsvpers'
        type: string
      - in: query
        name: repeat_rsvpers_min
        description: 'Positive Integer: Minumum range of the average number of repeat
          rsvpers'
        type: string
      - in: query
        name: rsvps_per_event_max
        description: 'Positive Integer: Maximum range of the average number of RSVPs
          per event'
        type: string
      - in: query
        name: rsvps_per_event_min
        description: 'Positive Integer: Minumum range of the average number of RSVPs
          per event'
        type: string
      - in: query
        name: topics
        description: 'List of Integers: the ids of topic of the group'
        type: string
      - in: query
        name: upcoming_events_max
        description: 'Positive Integer: Maximum range of the number of the upcoming
          events'
        type: string
      - in: query
        name: upcoming_events_min
        description: 'Positive Integer: Minumum range of the number of the upcoming
          events'
        type: string
      - in: query
        name: zip
        description: 'String: Zip code'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /pro/:urlname/members:
    get:
      summary: Search Pro Members
      description: Name, location, and time based search for the members of the meetups
        belonging to Pro organization.
      operationId: pro
      x-api-path-slug: prourlnamemembers-get
      parameters:
      - in: query
        name: active_within_days
        description: 'Positive Integer: The range of date from the past until today,
          for the recent activity'
        type: string
      - in: query
        name: chapters
        description: 'List of Integers: The chapters which the member belongs to'
        type: string
      - in: query
        name: country
        description: 'String: Country'
        type: string
      - in: query
        name: desc
        description: 'Boolean: whether to sort ascending or decending'
        type: string
      - in: query
        name: email_received
        description: 'Integers: The id of a previous emails that the member received'
        type: string
      - in: query
        name: events_attended_max
        description: 'Positive Integer: Maximum number of attended events'
        type: string
      - in: query
        name: events_attended_min
        description: 'Positive Integer: Minimum number of attended events'
        type: string
      - in: query
        name: is_organizer
        description: 'Boolean: To limit to only organizers or non-organizers'
        type: string
      - in: query
        name: join_time_max
        description: 'Milliseconds since epoch: The latest time limit for member join'
        type: string
      - in: query
        name: join_time_min
        description: 'Milliseconds since epoch: The oldest time limit for member join'
        type: string
      - in: query
        name: lat
        description: 'Float: Latitude'
        type: string
      - in: query
        name: location
        description: 'String: Raw location'
        type: string
      - in: query
        name: lon
        description: 'Float: Longitude'
        type: string
      - in: query
        name: member_name
        description: 'String: Name of the member'
        type: string
      - in: query
        name: offset
        description: 'Positive Integer: the page offset'
        type: string
      - in: query
        name: order
        description: 'String: attribute to sort on'
        type: string
      - in: query
        name: page
        description: 'Positive Integer: the size of page window'
        type: string
      - in: query
        name: query
        description: 'String: raw query string to search from member name or city'
        type: string
      - in: query
        name: radius
        description: 'String: `global`, `smart`, or search radius in Float'
        type: string
      - in: query
        name: zip
        description: 'String: Zip code'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /members/:member_id:
    get:
      summary: Get Member Profile
      description: |-
        Gets Member Profiles.
        For Group Profiles, see [this endpoint](/meetup_api/docs/:urlname/members/:member_id)
      operationId: profiles
      x-api-path-slug: membersmember-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /:urlname/members/:member_id:
    get:
      summary: Get Group Member Profile
      description: |-
        Gets Group Profiles.
        For Member Profiles, see [this endpoint](/meetup_api/docs/members/:member_id)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-get
      parameters:
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    patch:
      summary: Edit Group Member Profile
      description: |-
        Edits Group Profiles.
        To fetch Group Member Profiles,
        see [this endpoint](/meetup_api/docs/:urlname/members/:member_id#get)
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-patch
      parameters:
      - in: query
        name: add_role
        description: Allows those with permission to assign one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: answer_{qid}
        description: Answers to questions from groups API join_info question fields
        type: string
      - in: query
        name: fields
        description: A comma-delimited string of optional response field names
        type: string
      - in: query
        name: intro
        description: Provides a Member an opportunity to tell the group about themselves,in
          at most 255 characters
        type: string
      - in: query
        name: photo_id
        description: Numeric id of the photo to use for this profile
        type: string
      - in: query
        name: remove_role
        description: Allows those with permission to remove one of the following roles:assistant_organizer,
          coorganizer, or event_organizer
        type: string
      - in: query
        name: title
        description: An organizer-defined title,in at most 255 characters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
    delete:
      summary: Delete Group Member Profile (Leave Group)
      description: Deletes a member's group profiles.
      operationId: profiles
      x-api-path-slug: urlnamemembersmember-id-delete
      parameters:
      - in: query
        name: exit_comment
        description: Optional message to the organizer when leaving
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups
  /recommended/group_topics:
    get:
      summary: Recommend Group Topics
      description: Recommends suggestions for group topics based on a text search
        or other topics
      operationId: topics
      x-api-path-slug: recommendedgroup-topics-get
      parameters:
      - in: query
        name: exclude_topics
        description: A comma-delimited list of topic ids to exclude from the recommendations
        type: string
      - in: query
        name: lang
        description: Defines a language preference for ordering results
        type: string
      - in: query
        name: other_topics
        description: A comma-delimited list of topic ids to inform recommendations
        type: string
      - in: query
        name: page
        description: Target number of recommendations to return
        type: string
      - in: query
        name: text
        description: Free form text search
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Recomendations
      - Groups
      - Topics
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