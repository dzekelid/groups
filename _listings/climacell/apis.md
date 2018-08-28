---
name: ClimaCell
x-slug: climacell
description: ClimaCell provides the most accurate weather data in the world by integrating
  proprietary data extracted from wireless networks and other new sensing technologies
  with data from traditional sensors. With 90% correlation to ground truth (vs. 50%
  using radar), it&rsquo;s the best you can get for your enterprise.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
x-kinRank: "9"
x-alexaRank: "617213"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/apis.md
specificationVersion: "0.14"
apis:
- name: ClimaCell API - Get Groups
  x-api-slug: groups-get
  description: |-
    ### List all Groups
    Page through a list of all your groups. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groups-get-openapi.md
- name: ClimaCell API - Post Groups
  x-api-slug: groups-post
  description: |-
    ### Create a Group

    Creates a new Group, and name it. The system attaches a unique ID to each group you create. This ID is used to refer to the group and manage it in the following ```groups``` API calls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groups-post-openapi.md
- name: ClimaCell API - Get Groups Group
  x-api-slug: groupsgroup-id-get
  description: |-
    ### Retrieve a Group

    Get a single group with its information by specifying its ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-get-openapi.md
- name: ClimaCell API - Put Groups Group
  x-api-slug: groupsgroup-id-put
  description: |-
    ### Update a Group

    Updates the name of a Group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-put-openapi.md
- name: ClimaCell API - Delete Groups Group
  x-api-slug: groupsgroup-id-delete
  description: |-
    ### Delete a Group

    Removes a Group with the ```group_id``` from the system. Note that the user information will be lost.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-delete-openapi.md
- name: ClimaCell API - Get Groups Group Members
  x-api-slug: groupsgroup-idmembers-get
  description: |-
    ### List all Group Members
    Page through a list of all members of a group with a ```group_id```. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-get-openapi.md
- name: ClimaCell API - Post Groups Group Members
  x-api-slug: groupsgroup-idmembers-post
  description: |-
    ### Create a Group Member

    Adds a member to a group with a ```group_id```. ???Make sure you provide an accurate email address and/or phone number or alerts will not be received by the member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-post-openapi.md
- name: ClimaCell API - Put Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-put
  description: |-
    ### Delete a Group Member
    Updates a member with the ```member_id``` to the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-put-openapi.md
- name: ClimaCell API - Delete Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-delete
  description: |-
    ### Delete a Group Member
    Removes a member with the ```member_id``` from the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-delete-openapi.md
- name: ClimaCell API - Get Groups Group
  x-api-slug: groupsgroup-id-get
  description: |-
    ### Retrieve a Group

    Get a single group with its information by specifying its ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-get-openapi.md
- name: ClimaCell API - Put Groups Group
  x-api-slug: groupsgroup-id-put
  description: |-
    ### Update a Group

    Updates the name of a Group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-put-openapi.md
- name: ClimaCell API - Delete Groups Group
  x-api-slug: groupsgroup-id-delete
  description: |-
    ### Delete a Group

    Removes a Group with the ```group_id``` from the system. Note that the user information will be lost.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-delete-openapi.md
- name: ClimaCell API - Get Groups Group Members
  x-api-slug: groupsgroup-idmembers-get
  description: |-
    ### List all Group Members
    Page through a list of all members of a group with a ```group_id```. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-get-openapi.md
- name: ClimaCell API - Post Groups Group Members
  x-api-slug: groupsgroup-idmembers-post
  description: |-
    ### Create a Group Member

    Adds a member to a group with a ```group_id```. ???Make sure you provide an accurate email address and/or phone number or alerts will not be received by the member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-post-openapi.md
- name: ClimaCell API - Put Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-put
  description: |-
    ### Delete a Group Member
    Updates a member with the ```member_id``` to the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-put-openapi.md
- name: ClimaCell API - Delete Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-delete
  description: |-
    ### Delete a Group Member
    Removes a member with the ```member_id``` from the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-delete-openapi.md
- name: ClimaCell API - Delete Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-delete
  description: |-
    ### Delete a Group Member
    Removes a member with the ```member_id``` from the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-delete-openapi.md
- name: ClimaCell API - Put Groups Group Members Member
  x-api-slug: groupsgroup-idmembersmember-id-put
  description: |-
    ### Delete a Group Member
    Updates a member with the ```member_id``` to the group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembersmember-id-put-openapi.md
- name: ClimaCell API - Post Groups Group Members
  x-api-slug: groupsgroup-idmembers-post
  description: |-
    ### Create a Group Member

    Adds a member to a group with a ```group_id```. ???Make sure you provide an accurate email address and/or phone number or alerts will not be received by the member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-post-openapi.md
- name: ClimaCell API - Get Groups Group Members
  x-api-slug: groupsgroup-idmembers-get
  description: |-
    ### List all Group Members
    Page through a list of all members of a group with a ```group_id```. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-idmembers-get-openapi.md
- name: ClimaCell API - Delete Groups Group
  x-api-slug: groupsgroup-id-delete
  description: |-
    ### Delete a Group

    Removes a Group with the ```group_id``` from the system. Note that the user information will be lost.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-delete-openapi.md
- name: ClimaCell API - Put Groups Group
  x-api-slug: groupsgroup-id-put
  description: |-
    ### Update a Group

    Updates the name of a Group with a ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-put-openapi.md
- name: ClimaCell API - Get Groups Group
  x-api-slug: groupsgroup-id-get
  description: |-
    ### Retrieve a Group

    Get a single group with its information by specifying its ```group_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Weather, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/climacell/groupsgroup-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://clickatell.api.gallery.streamdata.io
- type: x-api-stack
  url: http://climacell.stack.network
- type: x-blog
  url: https://www.climacell.co/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/climacell
- type: x-developer
  url: https://www.climacell.co/api/
- type: x-email
  url: info@climacell.co
- type: x-email
  url: support@climacell.co
- type: x-email
  url: sales@climacell.co
- type: x-faq
  url: https://developer.climacell.co/FAQ
- type: x-github
  url: https://github.com/climacell
- type: x-pricing
  url: https://developer.climacell.co/
- type: x-privacy-policy
  url: https://www.climacell.co/privacy/
- type: x-terms-of-service
  url: https://www.climacell.co/terms-of-service/
- type: x-twitter
  url: https://twitter.com/WeatherRevealed
- type: x-website
  url: https://www.climacell.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---