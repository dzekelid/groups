---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph Check Member Groups
  x-api-slug: microsoft-graph
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/checkMemberGroups
  tags: Checks, Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/mecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/mecheckmembergroups-post-openapi.md
- name: Microsoft Graph Check Member Groups
  x-api-slug: microsoft-graph
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/checkMemberGroups
  tags: Checks, Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/usersid--userprincipalnamecheckmembergroups-post-openapi.md
- name: Microsoft Graph Group Check Member Groups
  x-api-slug: microsoft-graph
  description: 'group: checkMemberGroups Check for membership in the specified list
    of groups. Returns from the list those groups of which the specified group has
    a direct or transitive membership.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/checkMemberGroups
  tags: Group, Checks, Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groupsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph Check Member Groups
  x-api-slug: microsoft-graph
  description: Check member groups Check for membership in a specified list of groups,
    and returns from that list those groups of which the specified user, group, or
    directory object is a member. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////directoryObjects/{id}/checkMemberGroups
  tags: Checks, Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/directoryobjectsidcheckmembergroups-post-openapi.md
- name: Microsoft Graph Get Member Groups
  x-api-slug: microsoft-graph
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/getMemberGroups
  tags: Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/megetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/megetmembergroups-post-openapi.md
- name: Microsoft Graph Get Member Groups
  x-api-slug: microsoft-graph
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/getMemberGroups
  tags: Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/usersid--userprincipalnamegetmembergroups-post-openapi.md
- name: Microsoft Graph Group Get Member Groups
  x-api-slug: microsoft-graph
  description: 'group: getMemberGroups Return all the groups that the specified group
    is a member of. The check is transitive, unlike reading the memberOf navigation
    property, which returns only the groups that the group is a direct member of.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/getMemberGroups
  tags: Group, , Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groupsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groupsidgetmembergroups-post-openapi.md
- name: Microsoft Graph Get Member Groups
  x-api-slug: microsoft-graph
  description: Get member groups Return all the groups that the specified user, group,
    or directory object is a member of. This function is transitive.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////directoryObjects/{id}/getMemberGroups
  tags: Member, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/directoryobjectsidgetmembergroups-post-openapi.md
- name: Microsoft Graph List Groups
  x-api-slug: microsoft-graph
  description: List groups List all the groups available in an organization, including
    but not limited to Office 365 Groups. The default properties of each group are
    returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups
  tags: List, Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/groups-get-openapi.md
- name: Microsoft Graph List Calendar Groups
  x-api-slug: microsoft-graph
  description: List calendarGroups Get the user's calendar groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendarGroups
  tags: List, Calendar, Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroups-get-openapi.md
- name: Microsoft Graph
  x-api-slug: microsoft-graph
  description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
    cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
    Graph simplifies queries that would otherwise be more complex. You can use Microsoft
    Graph to: Access data from multiple Microsoft cloud services, including Azure
    Active Directory, Exchange Online as part of Office 365, SharePoint, OneDrive,
    OneNote, and Planner. Navigate between entities and relationships. Access intelligence
    and insights from the Microsoft cloud (for commercial users).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/microsoft-graph/openapi.md
x-common:
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---