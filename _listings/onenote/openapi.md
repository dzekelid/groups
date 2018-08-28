---
swagger: "2.0"
x-collection-name: OneNote
x-complete: 1
info:
  title: One Note
  description: easily-capture-content-into-onenote-with-this-rest-api-
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
    post:
      summary: Post Sectiongroups Sectiongroupid Sectiongroups
      description: Post sectiongroups sectiongroupid sectiongroups.
      operationId: postSectiongroupsSectiongroupSectiongroups
      x-api-path-slug: sectiongroupssectiongroupidsectiongroups-post
      parameters:
      - in: query
        name: Content-Type
        description: 'Required: The type of content being sent'
      - in: path
        name: sectionGroupId
        description: Specifies the section group
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
    post:
      summary: Post Sectiongroups Sectiongroupid Sections
      description: Post sectiongroups sectiongroupid sections.
      operationId: postSectiongroupsSectiongroupSections
      x-api-path-slug: sectiongroupssectiongroupidsections-post
      parameters:
      - in: query
        name: Content-Type
        description: 'Required: The type of content being sent'
      - in: path
        name: sectionGroupId
        description: Specifies the section group
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
  /notebooks/{notebookId}/sectiongroups:
    get:
      summary: Get Notebooks Notebookid Sectiongroups
      description: Returns a collection of section groups within a specific notebook.
      operationId: getNotebooksNotebookSectiongroups
      x-api-path-slug: notebooksnotebookidsectiongroups-get
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
      - in: path
        name: notebookId
        description: Specifies the notebook
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
      - Notebooks
      - NotebookId
      - Sectiongroups
    parameters:
      summary: Parameters Notebooks Notebookid Sectiongroups
      description: Parameters notebooks notebookid sectiongroups.
      operationId: parametersNotebooksNotebookSectiongroups
      x-api-path-slug: notebooksnotebookidsectiongroups-parameters
      responses:
        200:
          description: OK
      tags:
      - Notebooks
      - NotebookId
      - Sectiongroups
    post:
      summary: Post Notebooks Notebookid Sectiongroups
      description: Creates a new section group in a notebook.
      operationId: postNotebooksNotebookSectiongroups
      x-api-path-slug: notebooksnotebookidsectiongroups-post
      parameters:
      - in: query
        name: Content-Type
        description: 'Required: The type of content being sent'
      - in: path
        name: notebookId
        description: Specifies the notebook
      responses:
        200:
          description: OK
      tags:
      - Notebooks
      - NotebookId
      - Sectiongroups
---