---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting X-related-model Contact Groups Contacts
  description: X-related-model contactgroups contactgroup contacts.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ContactGroups:
    get:
      summary: Get Contactgroups
      description: Get contactgroups.
      operationId: getContactgroups
      x-api-path-slug: contactgroups-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    post:
      summary: Post Contactgroups
      description: Post contactgroups.
      operationId: postContactgroups
      x-api-path-slug: contactgroups-post
      parameters:
      - in: body
        name: ContactGroups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    put:
      summary: Put Contactgroups
      description: Put contactgroups.
      operationId: putContactgroups
      x-api-path-slug: contactgroups-put
      parameters:
      - in: body
        name: ContactGroups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
    x-related-model:
      summary: X-related-model Contactgroups
      description: X-related-model contactgroups.
      operationId: x-related-modelContactgroups
      x-api-path-slug: contactgroups-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
  /ContactGroups/{ContactGroupID}:
    delete:
      summary: Delete Contact Groups
      description: Delete contactgroups contactgroup.
      operationId: deleteContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-delete
      parameters:
      - in: path
        name: ContactGroupID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
    get:
      summary: Get Contact Groups
      description: Get contactgroups contactgroup.
      operationId: getContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-get
      parameters:
      - in: path
        name: ContactGroupID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
    post:
      summary: Post Contact Groups
      description: Post contactgroups contactgroup.
      operationId: postContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-post
      parameters:
      - in: path
        name: ContactGroupID
      - in: body
        name: ContactGroups
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
    x-related-model:
      summary: X-related-model Contact Groups
      description: X-related-model contactgroups contactgroup.
      operationId: x-related-modelContactgroupsContactgroup
      x-api-path-slug: contactgroupscontactgroupid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
  /ContactGroups/{ContactGroupID}/Contacts:
    delete:
      summary: Delete Contact Groups Contacts
      description: Delete contactgroups contactgroup contacts.
      operationId: deleteContactgroupsContactgroupContacts
      x-api-path-slug: contactgroupscontactgroupidcontacts-delete
      parameters:
      - in: path
        name: ContactGroupID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
      - Contacts
    put:
      summary: Put Contact Groups Contacts
      description: Put contactgroups contactgroup contacts.
      operationId: putContactgroupsContactgroupContacts
      x-api-path-slug: contactgroupscontactgroupidcontacts-put
      parameters:
      - in: path
        name: ContactGroupID
      - in: body
        name: Contacts
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
      - Contacts
    x-related-model:
      summary: X-related-model Contact Groups Contacts
      description: X-related-model contactgroups contactgroup contacts.
      operationId: x-related-modelContactgroupsContactgroupContacts
      x-api-path-slug: contactgroupscontactgroupidcontacts-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
      - Contacts
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