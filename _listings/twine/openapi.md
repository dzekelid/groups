swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /group:
    get:
      summary: List groups
      description: Get a list of groups matching the specified filters.
      operationId: fetchGroups
      x-api-path-slug: group-get
      parameters:
      - in: query
        name: filter[name]
        description: Group name
      - in: query
        name: filter[organization]
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Groups
    post:
      summary: Create a group
      description: Create a group record.
      operationId: createGroup
      x-api-path-slug: group-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Group
  /group/{id}:
    get:
      summary: Get a group
      description: Get a group record by id.
      operationId: fetchGroup
      x-api-path-slug: groupid-get
      parameters:
      - in: path
        name: id
        description: Group identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Group