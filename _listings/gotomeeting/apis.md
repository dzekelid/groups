---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Meeting - Get groups
  x-api-slug: groups-get
  description: List all groups for an account. This API call is only available to
    users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groups-get-openapi.md
- name: Go To Meeting - Get attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyattendees-get-openapi.md
- name: Go To Meeting - Get historical meetings by group
  x-api-slug: groupsgroupkeyhistoricalmeetings-get
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: 'Go To Meeting - DEPRECATED: Get historical meetings by group'
  x-api-slug: groupsgroupkeymeetings-get
  description: 'DEPRECATED: Please use the new API calls ''Get historical meetings
    by group'' and ''Get upcoming meetings by group''. Get meetings for a specified
    group. Additional filters can be used to view only meetings within a specified
    date range. This API call is only available to users with the admin role.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeymeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeymeetings-get-openapi.md
- name: Go To Meeting - Get organizers by group
  x-api-slug: groupsgroupkeyorganizers-get
  description: Returns all the organizers within a specific group. This API call is
    only available to users with the admin role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyorganizers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyorganizers-get-openapi.md
- name: Go To Meeting - Create organizer in group
  x-api-slug: groupsgroupkeyorganizers-post
  description: Creates a new organizer and sends an email to the email address defined
    in request. This API call is only available to users with the admin role. You
    may also pass 'G2W' or 'G2T' or 'OPENVOICE' as productType variables, creating
    organizers for those products. A G2W or G2T organizer will also have access to
    G2M.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyorganizers-post-openapi.md
- name: Go To Meeting - Get upcoming meetings by group
  x-api-slug: groupsgroupkeyupcomingmeetings-get
  description: Get upcoming meetings for a specified group. This API call is only
    available to users with the admin role. This API call can be used only for groups
    with maximum 50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkeyupcomingmeetings-get-openapi.md
- name: SCIM - Get Groups
  x-api-slug: groups-get
  description: Queries multiple group identities in the organization domain. Filtering,
    sorting and pagination are available. This call requires the role ROLE_ORG_READ.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groups-get-openapi.md
- name: SCIM - Create Group
  x-api-slug: groups-post
  description: Creates a new organization group and adds it to the user domain. Member
    groups and member users must be in the organization. This call requires the role
    ROLE_ORG_WRITE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groups-post-openapi.md
- name: SCIM - Delete Group
  x-api-slug: groupsgroupkey-delete
  description: Deletes a group from the organization (but not from the account). The
    group must be in the organization. This call requires the role ROLE_ORG_WRITE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkey-delete-openapi.md
- name: SCIM - Get Group
  x-api-slug: groupsgroupkey-get
  description: Queries group details in the organization domain. This call requires
    the role ROLE_ORG_READ.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkey-get-openapi.md
- name: SCIM - Update Group
  x-api-slug: groupsgroupkey-patch
  description: Updates one or more values of an existing group without sending the
    full definition. Member groups and member users must be in the organization. This
    call requires the role ROLE_ORG_WRITE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkey-patch-openapi.md
- name: SCIM - Replace Group
  x-api-slug: groupsgroupkey-put
  description: Updates an existing group. The request must include the full group
    definition. To modify one or more values without sending the full definition,
    see "Update Group". Member groups and member users must be in the organization.
    This call requires the role ROLE_ORG_WRITE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//identity/v1
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/gotomeeting/groupsgroupkey-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.url.shortener.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gotomeeting.stack.network
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---