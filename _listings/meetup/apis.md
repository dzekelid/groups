---
name: Meetup
x-slug: meetup
description: Find Meetups so you can do more of what matters to you. Or create your
  own group and meet people near you who share your interests.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
x-kinRank: "9"
x-alexaRank: "902"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/apis.md
specificationVersion: "0.14"
apis:
- name: Meetup Groups
  x-api-slug: meetup
  description: Fetch information about Meetup Groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/groups
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2groups-get-openapi.md
- name: Meetup Members
  x-api-slug: meetup
  description: API method for accessing members of Meetup Groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////members
  tags: Events,Groups,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/members-get-openapi.md
- name: Meetup Members
  x-api-slug: meetup
  description: API method for accessing members of Meetup Groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/members
  tags: Events,Groups,Member
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2members-get-openapi.md
- name: Meetup Member Get
  x-api-slug: meetup
  description: Retrieve a single member
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/member/:id
  tags: Events,Groups,Member
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2memberid-get-openapi.md
- name: Meetup Member Edit
  x-api-slug: meetup
  description: Edit the authorized member's attributes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/member/:id
  tags: Events,Groups,Member
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2memberid-post-openapi.md
- name: Meetup Ratings v2
  x-api-slug: meetup
  description: API method for accessing Meetup comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/event_ratings
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2event-ratings-get-openapi.md
- name: Meetup Group Photo Upload
  x-api-slug: meetup
  description: Uploads a new Meetup Group photo. To change other Group settings use
    the [Group Edit](/meetup_api/docs/:urlname/#edit) endpoint
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/group_photo
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2group-photo-post-openapi.md
- name: Meetup Member Photo Upload
  x-api-slug: meetup
  description: Uploads a photo to be associated with a Member
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////2/member_photo
  tags: Events,Groups,Member
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/2member-photo-post-openapi.md
- name: Meetup Groups
  x-api-slug: meetup
  description: API method for accessing meetup groups
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////groups
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/groups-get-openapi.md
- name: Meetup Report Group
  x-api-slug: meetup
  description: Submits a new abuse report for a target group. Abuse reports will be
    followed up on by our Community Support team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/abuse_reports
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnameabuse-reports-post-openapi.md
- name: Meetup Find Groups
  x-api-slug: meetup
  description: Text, location, category and friend-based group searches
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////find/groups
  tags: Events,Search,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/findgroups-get-openapi.md
- name: Meetup Group Profile list
  x-api-slug: meetup
  description: Get a list of Meetup group members
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/members
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnamemembers-get-openapi.md
- name: Meetup Group Profile search
  x-api-slug: meetup
  description: |-
    Find group member profiles by name.
    Member's who very recently joined or left the group may not be immediately searchable
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////find/:urlname/members
  tags: Events,Groups,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/findurlnamemembers-get-openapi.md
- name: Meetup Get Group
  x-api-slug: meetup
  description: Fetches a Meetup group by urlname
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlname-get-openapi.md
- name: Meetup Group Edit
  x-api-slug: meetup
  description: Allows organizers to edit their Meetup group information. To change
    group topics, see the [add](/meetup_api/docs/:urlname/topics/#add) and [remove](/meetup_api/docs/:urlname/topics/#remove)
    topics endpoints. To change group photo use the [Group photo upload](/meetup_api/docs/2/group_photo/#create)
    endpoint. OAuth authenticated requests require an additional [group_edit](/meetup_api/auth/#oauth2-scopes)
    permission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlname-post-openapi.md
- name: Meetup Member groups
  x-api-slug: meetup
  description: |-
    Lists the authenticated member's groups in the order of leadership,
    next upcoming event, then alphabetical order by name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////self/groups
  tags: Events,Members,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/selfgroups-get-openapi.md
- name: Meetup Search Pro Groups
  x-api-slug: meetup
  description: Name and statistics range search for the meetup groups belonging to
    Pro organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////pro/:urlname/groups
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/prourlnamegroups-get-openapi.md
- name: Meetup Search Pro Members
  x-api-slug: meetup
  description: Name, location, and time based search for the members of the meetups
    belonging to Pro organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////pro/:urlname/members
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/prourlnamemembers-get-openapi.md
- name: Meetup Get Member Profile
  x-api-slug: meetup
  description: |-
    Gets Member Profiles.
    For Group Profiles, see [this endpoint](/meetup_api/docs/:urlname/members/:member_id)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////members/:member_id
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/membersmember-id-get-openapi.md
- name: Meetup Group Join
  x-api-slug: meetup
  description: This method allows an authenticated member to join a group by creating
    a profile
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/members
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnamemembers-post-openapi.md
- name: Meetup Get Group Member Profile
  x-api-slug: meetup
  description: |-
    Gets Group Profiles.
    For Member Profiles, see [this endpoint](/meetup_api/docs/members/:member_id)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/members/:member_id
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnamemembersmember-id-get-openapi.md
- name: Meetup Edit Group Member Profile
  x-api-slug: meetup
  description: |-
    Edits Group Profiles.
    To fetch Group Member Profiles,
    see [this endpoint](/meetup_api/docs/:urlname/members/:member_id#get)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/members/:member_id
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnamemembersmember-id-patch-openapi.md
- name: Meetup Delete Group Member Profile (Leave Group)
  x-api-slug: meetup
  description: Deletes a member's group profiles.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/members/:member_id
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnamemembersmember-id-delete-openapi.md
- name: Meetup Recommend Group Topics
  x-api-slug: meetup
  description: Recommends suggestions for group topics based on a text search or other
    topics
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////recommended/group_topics
  tags: Events,Recomendations,Groups,Topics
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/recommendedgroup-topics-get-openapi.md
- name: Meetup Recommended Groups
  x-api-slug: meetup
  description: Returns groups Meetup finds relevant to you
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////recommended/groups
  tags: Events,Recomendations,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/recommendedgroups-get-openapi.md
- name: Meetup Recommended Groups Ignore
  x-api-slug: meetup
  description: Provides a form of feedback by requesting to remove a group from future
    recommendations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////recommended/groups/ignores/:urlname
  tags: Events,Recomendations,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/recommendedgroupsignoresurlname-post-openapi.md
- name: Meetup Group Events
  x-api-slug: meetup
  description: Gets a listing of all Meetup Events hosted by a target group, in ascending
    order by default
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com////:urlname/events
  tags: Events,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/urlnameevents-get-openapi.md
- name: Meetup
  x-api-slug: meetup
  description: Find Meetups so you can do more of what matters to you. Or create your
    own group and meet people near you who share your interests.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/6564-meetup.jpg
  humanURL: http://meetup.com
  baseURL: https://api.meetup.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/meetup/openapi.md
x-common:
- type: x-base
  url: http://api.meetup.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/meetup
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-email
  url: privacy@meetup.com
- type: x-email
  url: abuse@meetup.com
- type: x-email
  url: api_license@meetup.com
- type: x-email
  url: arbitration-opt-out@meetup.com
- type: x-email
  url: legal@meetup.com
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-twitter
  url: https://twitter.com/Meetup
- type: x-website
  url: http://meetup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---