---
swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Accounting
  description: -introductionthe-xero-accounting-api-is-a-restful-web-service-and-uses-the-oauth-v1-0a-protocol-to-authenticate-3rd-party-applications--the-accounting-api-exposes-accounting-and-related-functions-of-the-main-xero-application-and-can-be-used-for-a-variety-of-purposes-such-as-creating-transactions-like-invoices-and-credit-notes-right-through-to-extracting-accounting-data-via-our-reports-endpoint-
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
  /ContactGroups/{ContactGroupID}/Contacts/{ContactID}:
    delete:
      summary: Delete Contact Groups Contacts Contact
      description: Delete contactgroups contactgroup contacts contact.
      operationId: deleteContactgroupsContactgroupContactsContact
      x-api-path-slug: contactgroupscontactgroupidcontactscontactid-delete
      parameters:
      - in: path
        name: ContactGroupID
      - in: path
        name: ContactID
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
      - Contacts
      - ContactID
    x-related-model:
      summary: X-related-model Contact Groups Contacts Contact
      description: X-related-model contactgroups contactgroup contacts contact.
      operationId: x-related-modelContactgroupsContactgroupContactsContact
      x-api-path-slug: contactgroupscontactgroupidcontactscontactid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - ContactGroups
      - ContactGroupID
      - Contacts
      - ContactID
---