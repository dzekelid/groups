---
swagger: "2.0"
x-collection-name: OneNote
x-complete: 0
info:
  title: One Note Parameters Sectiongroups
  description: Parameters sectiongroups.
  version: 1.0.0
host: www.onenote.com
basePath: /api/v1.0/me/notes/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sectionGroups/{sectionGroupId}/sectionGroups:
    get:
      summary: Get Sectiongroups Sectiongroupid Sectiongroups
      description: Returns a collection of section groups within a specific section
        group.
      operationId: getSectiongroupsSectiongroupSectiongroups
      x-api-path-slug: sectiongroupssectiongroupidsectiongroups-get
      parameters:
      - in: query
        name: count
        description: true, to return the number of entities in the collection
      - in: query
        name: expand
        description: The navigation properties (sections, sectionGroups, parentNotebook,
          or parentSectionGroup) to return inline in the response
      - in: query
        name: filter
        description: The filter for the query
      - in: query
        name: orderby
        description: The property to order by
      - in: path
        name: sectionGroupId
        description: Specifies the section group
      - in: query
        name: select
        description: The properties to return
      - in: query
        name: skip
        description: The number of entities to skip in the result set
      - in: query
        name: top
        description: The number of entities to return from the result set
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
      - SectionGroups
    parameters:
      summary: Parameters Sectiongroups Sectiongroupid Sectiongroups
      description: Parameters sectiongroups sectiongroupid sectiongroups.
      operationId: parametersSectiongroupsSectiongroupSectiongroups
      x-api-path-slug: sectiongroupssectiongroupidsectiongroups-parameters
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
      - SectionGroups
  /sectionGroups/{sectionGroupId}/sections:
    get:
      summary: Get Sectiongroups Sectiongroupid Sections
      description: Returns a collection of sections within a specific section group.
      operationId: getSectiongroupsSectiongroupSections
      x-api-path-slug: sectiongroupssectiongroupidsections-get
      parameters:
      - in: query
        name: count
        description: true, to return the number of entities in the collection
      - in: query
        name: expand
        description: The navigation properties (parentNotebook or parentSectionGroup)
          to return inline in the response
      - in: query
        name: filter
        description: The filter for the query
      - in: query
        name: orderby
        description: The property to order by
      - in: path
        name: sectionGroupId
        description: Specifies the section group
      - in: query
        name: select
        description: The properties to return
      - in: query
        name: skip
        description: The number of entities to skip in the result set
      - in: query
        name: top
        description: The number of entities to return from the result set
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
      - Sections
    parameters:
      summary: Parameters Sectiongroups Sectiongroupid Sections
      description: Parameters sectiongroups sectiongroupid sections.
      operationId: parametersSectiongroupsSectiongroupSections
      x-api-path-slug: sectiongroupssectiongroupidsections-parameters
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
      - Sections
  /sectionGroups/{sectionGroupId}:
    get:
      summary: Get Sectiongroups Sectiongroupid
      description: Returns a specific section group object.
      operationId: getSectiongroupsSectiongroup
      x-api-path-slug: sectiongroupssectiongroupid-get
      parameters:
      - in: query
        name: expand
        description: The navigation properties (sections, sectionGroups, parentNotebook,
          or parentSectionGroup) to return inline in the response
      - in: path
        name: sectionGroupId
        description: Specifies the specific section group
      - in: query
        name: select
        description: The properties to return
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
    parameters:
      summary: Parameters Sectiongroups Sectiongroupid
      description: Parameters sectiongroups sectiongroupid.
      operationId: parametersSectiongroupsSectiongroup
      x-api-path-slug: sectiongroupssectiongroupid-parameters
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
      - SectionGroupId
  /sectionGroups/:
    get:
      summary: Get Sectiongroups
      description: Returns a collection of section groups.
      operationId: getSectiongroups
      x-api-path-slug: sectiongroups-get
      parameters:
      - in: query
        name: count
        description: true, to return the number of entities in the collection
      - in: query
        name: expand
        description: The navigation properties (sections, sectionGroups, parentNotebook,
          or parentSectionGroup) to return inline in the response
      - in: query
        name: filter
        description: The filter for the query
      - in: query
        name: orderby
        description: The property to order by
      - in: query
        name: select
        description: The properties to return
      - in: query
        name: skip
        description: The number of entities to skip in the result set
      - in: query
        name: top
        description: The number of entities to return from the result set
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
    parameters:
      summary: Parameters Sectiongroups
      description: Parameters sectiongroups.
      operationId: parametersSectiongroups
      x-api-path-slug: sectiongroups-parameters
      responses:
        200:
          description: OK
      tags:
      - SectionGroups
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