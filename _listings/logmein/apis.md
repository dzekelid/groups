---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToMeeting - Groups
  x-api-slug: groups-get
  description: List all groups for an account. This API call is only available to
    users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groups-get-openapi.md
- name: GoToMeeting - Upcoming meetings by group
  x-api-slug: groupsgroupkeyupcomingmeetings-get
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-openapi.md
- name: GoToMeeting - Organizers by group
  x-api-slug: groupsgroupkeyorganizers-get
  description: Returns all the organizers within a specific group. This API call is
    only available to users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-openapi.md
- name: GoToMeeting - Attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-openapi.md
- name: GoToMeeting - Organizer in group
  x-api-slug: groupsgroupkeyorganizers-post
  description: "Creates a new organizer and sends an email to the email address defined
    in request. This API call is only available to users with the admin role. You
    may also pass 'G2W' or 'G2T' or 'OPENVOICE' as productType variables, creating
    organizers for those products. A G2W or G2T organizer will also have access to
    G2M.\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"organizerEmail\"\t\t\t\"valid.org@email.com\"\t\t\tString
    with valid email syntax\t\t\r\n\t\t\"firstName\"\t\t\t\"First\"\t\t\tString -
    max 25 characters\t\t\r\n\t\t\"lastName\"\t\t\t\"Last\"\t\t\tString - max 25 characters\t\t\r\n\t\t\"productType\"\t\t\t\"G2M\"\t\t\tMust
    be: G2M, G2W, G2T, OV"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-post-openapi.md
- name: GoToMeeting - Historical meetings by group
  x-api-slug: groupsgroupkeyhistoricalmeetings-get
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: GoToMeeting - Historical meetings by group
  x-api-slug: groupsgroupkeyhistoricalmeetings-get
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: GoToMeeting - Historical meetings by group
  x-api-slug: groupsgroupkeyhistoricalmeetings-get
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: GoToMeeting - Organizer in group
  x-api-slug: groupsgroupkeyorganizers-post
  description: "Creates a new organizer and sends an email to the email address defined
    in request. This API call is only available to users with the admin role. You
    may also pass 'G2W' or 'G2T' or 'OPENVOICE' as productType variables, creating
    organizers for those products. A G2W or G2T organizer will also have access to
    G2M.\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"organizerEmail\"\t\t\t\"valid.org@email.com\"\t\t\tString
    with valid email syntax\t\t\r\n\t\t\"firstName\"\t\t\t\"First\"\t\t\tString -
    max 25 characters\t\t\r\n\t\t\"lastName\"\t\t\t\"Last\"\t\t\tString - max 25 characters\t\t\r\n\t\t\"productType\"\t\t\t\"G2M\"\t\t\tMust
    be: G2M, G2W, G2T, OV"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-post-openapi.md
- name: GoToMeeting - Organizer in group
  x-api-slug: groupsgroupkeyorganizers-post
  description: "Creates a new organizer and sends an email to the email address defined
    in request. This API call is only available to users with the admin role. You
    may also pass 'G2W' or 'G2T' or 'OPENVOICE' as productType variables, creating
    organizers for those products. A G2W or G2T organizer will also have access to
    G2M.\r\n\t\t\t\t\t\t\t\t\t\t\r\n\t\tfield\t\t\tvalue\t\t\tdescription\t\t\r\n\t\t\"organizerEmail\"\t\t\t\"valid.org@email.com\"\t\t\tString
    with valid email syntax\t\t\r\n\t\t\"firstName\"\t\t\t\"First\"\t\t\tString -
    max 25 characters\t\t\r\n\t\t\"lastName\"\t\t\t\"Last\"\t\t\tString - max 25 characters\t\t\r\n\t\t\"productType\"\t\t\t\"G2M\"\t\t\tMust
    be: G2M, G2W, G2T, OV"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-post-openapi.md
- name: GoToMeeting - Attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-openapi.md
- name: GoToMeeting - Attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyattendees-get-openapi.md
- name: GoToMeeting - Organizers by group
  x-api-slug: groupsgroupkeyorganizers-get
  description: Returns all the organizers within a specific group. This API call is
    only available to users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-openapi.md
- name: GoToMeeting - Organizers by group
  x-api-slug: groupsgroupkeyorganizers-get
  description: Returns all the organizers within a specific group. This API call is
    only available to users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyorganizers-get-openapi.md
- name: GoToMeeting - Upcoming meetings by group
  x-api-slug: groupsgroupkeyupcomingmeetings-get
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-openapi.md
- name: GoToMeeting - Upcoming meetings by group
  x-api-slug: groupsgroupkeyupcomingmeetings-get
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/logmein/groupsgroupkeyupcomingmeetings-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---