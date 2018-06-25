---
name: Learnifier
x-slug: learnifier
description: Create your online courses in minutes. Learnifier is the fast and easy
  tool for creating and sharing great courses that work on your mobile, tablet and
  desktop. Book a DEMO or test it out with our FREE TRIAL.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
x-kinRank: "7"
x-alexaRank: "5836977"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/apis.md
specificationVersion: "0.14"
apis:
- name: Learnifier List Global User Groups.
  x-api-slug: learnifier
  description: Returns a list of Global User Groups. Global User Groups are set up
    for the realm, and will generate groups that can be used on the client level.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////globalusergroups
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/globalusergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/globalusergroups-get-openapi.md
- name: Learnifier List of all users in group.
  x-api-slug: learnifier
  description: Returns a list of all members in User Groups that are based on the
    Global Group with this groupid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////globalusergroups/{groupid}/members
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/globalusergroupsgroupidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/globalusergroupsgroupidmembers-get-openapi.md
- name: Learnifier List User Groups.
  x-api-slug: learnifier
  description: Returns a list of User Groups for the org unit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups
  tags: Organizations,Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroups-get-openapi.md
- name: Learnifier Create a User Group.
  x-api-slug: learnifier
  description: Create a User Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups
  tags: Organizations,Users,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroups-post-openapi.md
- name: Learnifier Get user group
  x-api-slug: learnifier
  description: Returns single User Group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups/{groupid}
  tags: Organizations,Users,Groups,Groupid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroupsgroupid-get-openapi.md
- name: Learnifier List of all users in group.
  x-api-slug: learnifier
  description: Returns a list of all members in User Groups that are based on the
    Global Group with this groupid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups/{groupid}/members
  tags: Organizations,Uses,Groups,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroupsgroupidmembers-get-openapi.md
- name: Learnifier Add user group member.
  x-api-slug: learnifier
  description: Adds a user to user group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups/{groupid}/members
  tags: Organizations,Uses,Groups,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroupsgroupidmembers-post-openapi.md
- name: Learnifier Remove user group member.
  x-api-slug: learnifier
  description: Removes a user from a user group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com////orgunits/{orgid}/usergroups/{groupid}/members/{uuid}
  tags: Organizations,Uses,Groups,Members
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/orgunitsorgidusergroupsgroupidmembersuuid-delete-openapi.md
- name: Learnifier
  x-api-slug: learnifier
  description: Create your online courses in minutes. Learnifier is the fast and easy
    tool for creating and sharing great courses that work on your mobile, tablet and
    desktop. Book a DEMO or test it out with our FREE TRIAL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28448-learnifier.jpg
  humanURL: http://learnifier.com
  baseURL: https://learnifier.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/learnifier/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/learnifier
- type: x-developer
  url: https://learnifier.com/api/
- type: x-email
  url: sales@learnifier.com
- type: x-email
  url: Abdalla.Mohamed@learnifier.com
- type: x-email
  url: support@learnifier.com
- type: x-email
  url: jerker.klang@learnifier.com
- type: x-email
  url: mattias.borg@learnifier.com
- type: x-email
  url: lars.peterstrand@learnifier.com
- type: x-email
  url: hello@learnifier.com
- type: x-email
  url: unsubscribe@learnifier.com
- type: x-email
  url: privacy@learnifier.com
- type: x-twitter
  url: https://twitter.com/Learnifier
- type: x-website
  url: http://learnifier.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---