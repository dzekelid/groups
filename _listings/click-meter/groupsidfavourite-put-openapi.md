---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Fast switch the "favourite" field of a group
  description: Fast switch the "favourite" field of a group.
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /aggregated/summary/groups:
    get:
      summary: Retrieve statistics about a subset of groups for a timeframe with groups
        data
      description: Retrieve statistics about a subset of groups for a timeframe with
        groups data.
      operationId: getAggregatedSummaryGroups
      x-api-path-slug: aggregatedsummarygroups-get
      parameters:
      - in: query
        name: favourite
        description: Is the group marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - Summary
      - Groups
  /groups:
    get:
      summary: List of all the groups associated to the user.
      description: List of all the groups associated to the user..
      operationId: getGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: status
        description: Status of the group
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: write
        description: Write permission
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Create a group
      description: Create a group.
      operationId: postGroups
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: value
        description: The body of the group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/aggregated:
    get:
      summary: Retrieve statistics about this customer for a timeframe by groups
      description: Retrieve statistics about this customer for a timeframe by groups.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsaggregated-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
  /groups/aggregated/list:
    get:
      summary: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
      - List
  /groups/count:
    get:
      summary: Count the groups associated to the user.
      description: Count the groups associated to the user..
      operationId: getGroupsCount
      x-api-path-slug: groupscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude groups created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude groups created after this date (YYYYMMDD)
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: write
        description: Write permission
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Count
  /groups/{id}:
    delete:
      summary: Delete group specified by id
      description: Delete group specified by id.
      operationId: deleteGroups
      x-api-path-slug: groupsid-delete
      parameters:
      - in: path
        name: id
        description: Id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
    get:
      summary: Get a group
      description: Get a group.
      operationId: getGroups
      x-api-path-slug: groupsid-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
    post:
      summary: Update a group
      description: Update a group.
      operationId: postGroups
      x-api-path-slug: groupsid-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: body
        name: value
        description: The body of the group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
  /groups/{id}/aggregated:
    get:
      summary: Retrieve statistics about this group for a timeframe
      description: Retrieve statistics about this group for a timeframe.
      operationId: getGroupsAggregated
      x-api-path-slug: groupsidaggregated-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: hourly
        description: If using yesterday or today timeframe you can ask for the hourly
          detail
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
  /groups/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this group for a timeframe grouped by some
        temporal entity (day/week/month)
      description: Retrieve statistics about this group for a timeframe grouped by
        some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - List
  /groups/{id}/aggregated/summary:
    get:
      summary: Retrieve statistics about a subset of datapoints for a timeframe with
        datapoints data
      description: Retrieve statistics about a subset of datapoints for a timeframe
        with datapoints data.
      operationId: getGroupsAggregatedSummary
      x-api-path-slug: groupsidaggregatedsummary-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: path
        name: id
        description: Filter by this group id
      - in: query
        name: limit
        description: Limit results to this number
      - in: query
        name: offset
        description: Offset where to start from
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - Summary
  /groups/{id}/datapoints:
    get:
      summary: List of all the datapoints associated to the user in this group.
      description: List of all the datapoints associated to the user in this group..
      operationId: getGroupsDatapoints
      x-api-path-slug: groupsiddatapoints-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: limit
        description: Maximum elements to retrieve
      - in: query
        name: offset
        description: Where to start when retrieving elements
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: sortBy
        description: Field to sort by
      - in: query
        name: sortDirection
        description: Direction of sort asc or desc
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
    post:
      summary: Create a datapoint in this group
      description: Create a datapoint in this group.
      operationId: postGroupsDatapoints
      x-api-path-slug: groupsiddatapoints-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: body
        name: value
        description: The body of the datapoint
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
  /groups/{id}/datapoints/count:
    get:
      summary: Count the datapoints associated to the user in this group.
      description: Count the datapoints associated to the user in this group..
      operationId: getGroupsDatapointsCount
      x-api-path-slug: groupsiddatapointscount-get
      parameters:
      - in: query
        name: createdAfter
        description: Exclude datapoints created before this date (YYYYMMDD)
      - in: query
        name: createdBefore
        description: Exclude datapoints created after this date (YYYYMMDD)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: onlyFavorites
        description: Filter fields by favourite status
      - in: query
        name: status
        description: Status of the datapoint
      - in: query
        name: tags
        description: A comma separated list of tags you want to filter with
      - in: query
        name: textSearch
        description: Filter fields by this pattern
      - in: query
        name: type
        description: Type of the datapoint (tp/tl)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Datapoints
      - Count
  /groups/{id}/favourite:
    put:
      summary: Fast switch the "favourite" field of a group
      description: Fast switch the "favourite" field of a group.
      operationId: putGroupsFavourite
      x-api-path-slug: groupsidfavourite-put
      parameters:
      - in: path
        name: id
        description: Id of the group
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Favourite
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---