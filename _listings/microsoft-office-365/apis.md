---
name: Microsoft Office 365
x-slug: microsoft-office-365
description: Integrate Office 365 REST APIs powered by Microsoft Graph into your own
  app to connect to files, calendars, mail and more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Office 365 Get Calendar Groups
  x-api-slug: microsoft-office-365
  description: You can request all the calendar groups in a mailbox (or a f...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups
  tags: Calendargroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroups-get-openapi.md
- name: Microsoft Office 365 Add Calendar Groups
  x-api-slug: microsoft-office-365
  description: You can create a calendar group by sending a POST request wi...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups
  tags: Calendargroups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroups-post-openapi.md
- name: Microsoft Office 365 Get Calendar Groups
  x-api-slug: microsoft-office-365
  description: Get calendargroups calendargroup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}
  tags: Calendargroups, Calendargroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-get-openapi.md
- name: Microsoft Office 365 Add Calendar Groups
  x-api-slug: microsoft-office-365
  description: Post calendargroups calendargroup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}
  tags: Calendargroups, Calendargroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-post-openapi.md
- name: Microsoft Office 365 Delete Calendar Groups
  x-api-slug: microsoft-office-365
  description: Deleting a calendar group is as simple as sending a DELETE r...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}
  tags: Calendargroups, Calendargroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-delete-openapi.md
- name: Microsoft Office 365 Patch Calendar Groups
  x-api-slug: microsoft-office-365
  description: You can update a calendar group by sending a PATCH request w...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}
  tags: Calendargroups, Calendargroup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-patch-openapi.md
- name: Microsoft Office 365 Parameters Calendar Groups
  x-api-slug: microsoft-office-365
  description: Parameters calendargroups calendargroup
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}
  tags: Calendargroups, Calendargroup
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-id-parameters-openapi.md
- name: Microsoft Office 365 Get Calendar Groups Calendars
  x-api-slug: microsoft-office-365
  description: You can request all the user's calendars (or a filtered list...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}/Calendars
  tags: Calendargroups, Calendargroup, , Calendars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-idcalendars-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-idcalendars-get-openapi.md
- name: Microsoft Office 365 Add Calendar Groups Calendars
  x-api-slug: microsoft-office-365
  description: You can create a calendar by sending a POST request with a J...
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}/Calendars
  tags: Calendargroups, Calendargroup, , Calendars
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-idcalendars-post-openapi.md
- name: Microsoft Office 365 Parameters Calendar Groups Calendars
  x-api-slug: microsoft-office-365
  description: Parameters calendargroups calendargroup  calendars
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me//CalendarGroups{calendargroup_id}/Calendars
  tags: Calendargroups, Calendargroup, , Calendars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-idcalendars-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/calendargroupscalendargroup-idcalendars-parameters-openapi.md
- name: Microsoft Office 365
  x-api-slug: microsoft-office-365
  description: Integrate Office 365 REST APIs powered by Microsoft Graph into your
    own app to connect to files, calendars, mail and more.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-office.png
  humanURL: http://office.com
  baseURL: https://outlook.office365.com//ews/odata/Me
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-office-365/openapi.md
x-common:
- type: x-developer
  url: http://dev.office.com
- type: x-github
  url: https://github.com/OfficeDev
- type: x-twitter
  url: https://twitter.com/OfficeDev
- type: x-website
  url: http://office.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---