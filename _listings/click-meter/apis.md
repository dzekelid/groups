---
name: Click Meter
x-slug: click-meter
description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
  agency. The ClickMeter System was initially a web tool created to address the needs
  of our agency to precisely count and track the web-marketing actions we performed
  for our customers.The system evolved rapidly, and emerged as one of the most widely
  used software solutions in our agency to collect, analyze, and share data for and
  with our customers. After few years after the development of the first ClickMeter
  system, we decided to go live with a service that can be useful to everyone involved
  in web-marketing activities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/apis.md
specificationVersion: "0.14"
apis:
- name: Click Meter Retrieve statistics about a subset of groups for a timeframe with
    groups data
  x-api-slug: click-meter
  description: Retrieve statistics about a subset of groups for a timeframe with groups
    data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////aggregated/summary/groups
  tags: Aggregated,Summary,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/aggregatedsummarygroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/aggregatedsummarygroups-get-openapi.md
- name: Click Meter List of all the groups associated to the user.
  x-api-slug: click-meter
  description: List of all the groups associated to the user..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groups-get-openapi.md
- name: Click Meter Create a group
  x-api-slug: click-meter
  description: Create a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groups-post-openapi.md
- name: Click Meter Retrieve statistics about this customer for a timeframe by groups
  x-api-slug: click-meter
  description: Retrieve statistics about this customer for a timeframe by groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/aggregated
  tags: Groups,Aggregated
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsaggregated-get-openapi.md
- name: Click Meter Retrieve statistics about all groups of this customer for a timeframe
    grouped by some temporal entity (day/week/month)
  x-api-slug: click-meter
  description: Retrieve statistics about all groups of this customer for a timeframe
    grouped by some temporal entity (day/week/month).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/aggregated/list
  tags: Groups,Aggregated,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsaggregatedlist-get-openapi.md
- name: Click Meter Count the groups associated to the user.
  x-api-slug: click-meter
  description: Count the groups associated to the user..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/count
  tags: Groups,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupscount-get-openapi.md
- name: Click Meter Delete group specified by id
  x-api-slug: click-meter
  description: Delete group specified by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}
  tags: Groups,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsid-delete-openapi.md
- name: Click Meter Get a group
  x-api-slug: click-meter
  description: Get a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}
  tags: Groups,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsid-get-openapi.md
- name: Click Meter Update a group
  x-api-slug: click-meter
  description: Update a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}
  tags: Groups,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsid-post-openapi.md
- name: Click Meter Retrieve statistics about this group for a timeframe
  x-api-slug: click-meter
  description: Retrieve statistics about this group for a timeframe.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/aggregated
  tags: Groups,Id,Aggregated
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidaggregated-get-openapi.md
- name: Click Meter Retrieve statistics about this group for a timeframe grouped by
    some temporal entity (day/week/month)
  x-api-slug: click-meter
  description: Retrieve statistics about this group for a timeframe grouped by some
    temporal entity (day/week/month).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/aggregated/list
  tags: Groups,Id,Aggregated,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidaggregatedlist-get-openapi.md
- name: Click Meter Retrieve statistics about a subset of datapoints for a timeframe
    with datapoints data
  x-api-slug: click-meter
  description: Retrieve statistics about a subset of datapoints for a timeframe with
    datapoints data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/aggregated/summary
  tags: Groups,Id,Aggregated,Summary
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidaggregatedsummary-get-openapi.md
- name: Click Meter List of all the datapoints associated to the user in this group.
  x-api-slug: click-meter
  description: List of all the datapoints associated to the user in this group..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/datapoints
  tags: Groups,Id,Datapoints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsiddatapoints-get-openapi.md
- name: Click Meter Create a datapoint in this group
  x-api-slug: click-meter
  description: Create a datapoint in this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/datapoints
  tags: Groups,Id,Datapoints
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsiddatapoints-post-openapi.md
- name: Click Meter Count the datapoints associated to the user in this group.
  x-api-slug: click-meter
  description: Count the datapoints associated to the user in this group..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/datapoints/count
  tags: Groups,Id,Datapoints,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsiddatapointscount-get-openapi.md
- name: Click Meter Fast switch the "favourite" field of a group
  x-api-slug: click-meter
  description: Fast switch the "favourite" field of a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/favourite
  tags: Groups,Id,Favourite
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidfavourite-put-openapi.md
- name: Click Meter Retrieve the list of events related to this group.
  x-api-slug: click-meter
  description: Retrieve the list of events related to this group..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/hits
  tags: Groups,Id,Hits
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidhits-get-openapi.md
- name: Click Meter Fast patch the "notes" field of a group
  x-api-slug: click-meter
  description: Fast patch the "notes" field of a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/notes
  tags: Groups,Id,Notes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidnotes-put-openapi.md
- name: Click Meter Retrieve a top report connected to this group
  x-api-slug: click-meter
  description: Retrieve a top report connected to this group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////groups/{id}/reports
  tags: Groups,Id,Reports
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/groupsidreports-get-openapi.md
- name: Click Meter Delete the association of this tag with all groups
  x-api-slug: click-meter
  description: Delete the association of this tag with all groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups
  tags: Tags,TagId,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/tagstagidgroups-delete-openapi.md
- name: Click Meter List of all the groups associated to the user filtered by this
    tag.
  x-api-slug: click-meter
  description: List of all the groups associated to the user filtered by this tag..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups
  tags: Tags,TagId,Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/tagstagidgroups-get-openapi.md
- name: Click Meter Count the groups associated to the user filtered by this tag
  x-api-slug: click-meter
  description: Count the groups associated to the user filtered by this tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups/count
  tags: Tags,TagId,Groups,Count
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/tagstagidgroupscount-get-openapi.md
- name: Click Meter Associate/Deassociate a tag with a group
  x-api-slug: click-meter
  description: Associate/deassociate a tag with a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80////tags/{tagId}/groups/patch
  tags: Tags,TagId,Groups,Patch
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/tagstagidgroupspatch-put-openapi.md
- name: Click Meter
  x-api-slug: click-meter
  description: ClickMeter was founded in 2012 as a byproduct of an experienced web-marketing
    agency. The ClickMeter System was initially a web tool created to address the
    needs of our agency to precisely count and track the web-marketing actions we
    performed for our customers.The system evolved rapidly, and emerged as one of
    the most widely used software solutions in our agency to collect, analyze, and
    share data for and with our customers. After few years after the development of
    the first ClickMeter system, we decided to go live with a service that can be
    useful to everyone involved in web-marketing activities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clickmeter-logo.png
  humanURL: http://clickmeter.com
  baseURL: https://apiv2.clickmeter.com:80//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/click-meter/openapi.md
x-common:
- type: x-blog
  url: https://blog.clickmeter.com/
- type: x-pricing
  url: http://clickmeter.com/pricing-signup
- type: x-support
  url: https://support.clickmeter.com/hc/en-us
- type: x-terms-of-service
  url: http://clickmeter.com/terms-conditions
- type: x-twitter
  url: https://twitter.com/clickmeter
- type: x-website
  url: http://clickmeter.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---