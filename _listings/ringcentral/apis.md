---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Get User Groups
  x-api-slug: restapiv1-0glipgroups-get
  description: |-
    Returns the list of groups associated with the user.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroups-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Groups
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroups-get
  description: |-
    Returns call monitoring groups that can be filtered by some extension.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroups-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Group
  x-api-slug: restapiv1-0glipgroups-post
  description: |-
    Creates a group.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroups-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group
  x-api-slug: restapiv1-0glipgroupsgroupid-get
  description: |-
    Returns a group or multiple groups by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Group Members
  x-api-slug: restapiv1-0glipgroupsgroupidbulkassign-post
  description: |-
    Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group Posts
  x-api-slug: restapiv1-0glipgroupsgroupidposts-get
  description: |-
    Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Post in Group
  x-api-slug: restapiv1-0glipgroupsgroupidposts-post
  description: |-
    Creates a new post in a group specified.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Webhook in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-post
  description: |-
    Create new Webhook
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhooks in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-get
  description: |-
    Returns webhooks which are available for the current user (by group ID).
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Users
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get
  description: "Returns the list of users allowed to page this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
  description: "Returns the list of paging devices assigned to this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyDevices\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Paging Group Users and Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Call Queue Group
  x-api-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
  description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser Permission\nGroups\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nEXT-405\nExtension of type [ParkLocation] could not be
    a member of [department}]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Group Members
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
  description: |-
    Returns call monitoring group members.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Group Members
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
  description: |-
    Returns call monitoring group members.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Group Members
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
  description: |-
    Returns call monitoring group members.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Call Queue Group
  x-api-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
  description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser Permission\nGroups\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nEXT-405\nExtension of type [ParkLocation] could not be
    a member of [department}]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Call Queue Group
  x-api-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
  description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser Permission\nGroups\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nEXT-405\nExtension of type [ParkLocation] could not be
    a member of [department}]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Paging Group Users and Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Paging Group Users and Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Paging Group Users and Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
  description: "Returns the list of paging devices assigned to this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyDevices\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
  description: "Returns the list of paging devices assigned to this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyDevices\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
  description: "Returns the list of paging devices assigned to this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyDevices\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Users
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get
  description: "Returns the list of users allowed to page this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Users
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get
  description: "Returns the list of users allowed to page this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhooks in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-get
  description: |-
    Returns webhooks which are available for the current user (by group ID).
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhooks in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-get
  description: |-
    Returns webhooks which are available for the current user (by group ID).
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Webhook in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-post
  description: |-
    Create new Webhook
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Webhook in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-post
  description: |-
    Create new Webhook
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Post in Group
  x-api-slug: restapiv1-0glipgroupsgroupidposts-post
  description: |-
    Creates a new post in a group specified.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Post in Group
  x-api-slug: restapiv1-0glipgroupsgroupidposts-post
  description: |-
    Creates a new post in a group specified.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group Posts
  x-api-slug: restapiv1-0glipgroupsgroupidposts-get
  description: |-
    Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group Posts
  x-api-slug: restapiv1-0glipgroupsgroupidposts-get
  description: |-
    Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Group Members
  x-api-slug: restapiv1-0glipgroupsgroupidbulkassign-post
  description: |-
    Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Group Members
  x-api-slug: restapiv1-0glipgroupsgroupidbulkassign-post
  description: |-
    Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group
  x-api-slug: restapiv1-0glipgroupsgroupid-get
  description: |-
    Returns a group or multiple groups by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group
  x-api-slug: restapiv1-0glipgroupsgroupid-get
  description: |-
    Returns a group or multiple groups by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroupsgroupid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Group
  x-api-slug: restapiv1-0glipgroups-post
  description: |-
    Creates a group.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroups-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Group
  x-api-slug: restapiv1-0glipgroups-post
  description: |-
    Creates a group.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ringcentral/restapiv1-0glipgroups-post-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---