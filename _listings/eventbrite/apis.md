---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite brings people together through live experiences. Discover
  events that match your passions, or create your own with online ticketing tools.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
x-kinRank: "9"
x-alexaRank: "643"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Get Events Event Ticket Groups
  x-api-slug: eventbrite
  description: |-
    Get the list of ticket_group for the event with the specified :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///events/:event_id/ticket_groups/
  tags: Events,:event,Ticket,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-groups-get-openapi.md
- name: Eventbrite Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
    Group
  x-api-slug: eventbrite
  description: Add the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id to the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/
  tags: Events,:event,Ticket,Classes,:ticket,Class,Ticket,Groups,:ticket,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-openapi.md
- name: Eventbrite Delete Events Event Ticket Classes Ticket Class Ticket Groups Ticket
    Group
  x-api-slug: eventbrite
  description: Remove the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id from the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/
  tags: Events,:event,Ticket,Classes,:ticket,Class,Ticket,Groups,:ticket,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-openapi.md
- name: Eventbrite Get Events Event Ticket Classes Ticket Class Ticket Groups
  x-api-slug: eventbrite
  description: |-
    Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/
  tags: Events,:event,Ticket,Classes,:ticket,Class,Ticket,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-openapi.md
- name: Eventbrite Get Ticket Groups Ticket Group
  x-api-slug: eventbrite
  description: Returns the ticket_group with the specified :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///ticket_groups/:ticket_group_id/
  tags: Ticket,Groups,:ticket,Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/ticket-groupsticket-group-id-get-openapi.md
- name: Eventbrite Delete Ticket Groups Ticket Group
  x-api-slug: eventbrite
  description: |-
    Deletes the ticket_group with the specified :ticket_group_id.
    The status of the ticket group is changed to deleted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///ticket_groups/:ticket_group_id/
  tags: Ticket,Groups,:ticket,Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/ticket-groupsticket-group-id-delete-openapi.md
- name: Eventbrite Post Ticket Groups
  x-api-slug: eventbrite
  description: |-
    Creates a ticket group and returns the created ticket_group.
    Only up to 200 live ticket groups may be created; those with archived or deleted status are not taken into account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///ticket_groups/
  tags: Ticket,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/ticket-groups-post-openapi.md
- name: Eventbrite Post Ticket Groups Ticket Group
  x-api-slug: eventbrite
  description: Updates the ticket group with the specified :ticket_group_id. Returns
    the updated ticket_group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///ticket_groups/:ticket_group_id/
  tags: Ticket,Groups,:ticket,Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/ticket-groupsticket-group-id-post-openapi.md
- name: Eventbrite Get Users User Ticket Groups
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of ticket_group for the specified user.
    The alias me (/users/me/) may be used to refer to the currently authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/ticket_groups/
  tags: Users,:user,Ticket,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/usersuser-idticket-groups-get-openapi.md
- name: Eventbrite Post Users User Events Event Ticket Classes Ticket Class Ticket
    Groups
  x-api-slug: eventbrite
  description: |-
    Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
    belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
    If the list provided is empty, remove this ticket class from every ticket group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/
  tags: Users,:user,Events,:event,Ticket,Classes,:ticket,Class,Ticket,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite brings people together through live experiences. Discover
    events that match your passions, or create your own with online ticketing tools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-crunchbase
  url: https://crunchbase.com/organization/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-twitter
  url: https://twitter.com/eventbrite
- type: x-website
  url: http://eventbriteapi.com
- type: x-website
  url: http://developer.eventbrite.com/
- type: x-website
  url: http://eventbrite.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---