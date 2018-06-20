---
swagger: "2.0"
x-collection-name: BBC
x-complete: 0
info:
  title: BBC Nitro Get raw genre groups
  description: Get raw genre groups
  termsOfService: http://www.bbc.co.uk/terms/
  contact:
    name: Open Nitro Project
    url: http://developer.bbc.co.uk/
    email: nitro@bbc.co.uk
  version: 1.0.0
host: programmes.api.bbc.com
basePath: /nitro/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    get:
      summary: 'Find metadata for curated groups: seasons, collections, galleries
        or franchises'
      description: Long-lived curated collections of programmes and more, including
        Collections, Seasons, Franchises and Galleries
      operationId: listGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: embargoed
        description: Control return of embargoed items (undocumented)
      - in: query
        name: for_descendants_of
        description: filter for groups related to given programme or its descendants
      - in: query
        name: for_programme
        description: filter for subset of groups directly related to a given programme
      - in: query
        name: group
        description: filter for subset of groups which belong to the given group pid
      - in: query
        name: group_type
        description: filter for subset of groups that have the given group type
      - in: query
        name: member
        description: filter for subset of groups which contain an entity with the
          given pid as a member
      - in: query
        name: mixin
        description: 'Mixins:* alternate_images: mixin to return the alternate images
          for a group* group_for: mixin to return links to programme entities that
          group belongs to* images: mixin to add image information for a group* related_links:
          mixin to return related links for the group'
      - in: query
        name: page
        description: which page of results to return
      - in: query
        name: page_size
        description: number of results in each page
      - in: query
        name: partner_id
        description: filter for groups by partner ID
      - in: query
        name: partner_pid
        description: filter for groups by partner PID
      - in: query
        name: pid
        description: filter for subset of seasons, collections, galleries or franchises
          having given PID
      - in: query
        name: q
        description: filter for subset of groups matching supplied keyword/phrase
          (boolean operators permitted)
      - in: query
        name: sort
        description: 'Sorts:* pid: sort alphabetically by PID'
      - in: query
        name: sort_direction
        description: Sort direction
      responses:
        200:
          description: OK
      tags:
      - Groups
  /v1/episodes/{pid}/genre_groups/:
    get:
      summary: Get raw genre groups
      description: Get raw genre groups
      operationId: Get_Raw_genre_groups
      x-api-path-slug: v1episodespidgenre-groups-get
      parameters:
      - in: path
        name: pid
      responses:
        200:
          description: OK
      tags:
      - V1
      - Episodes
      - Pid
      - Genre
      - Groups
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