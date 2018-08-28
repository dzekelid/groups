swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hsmGroups:
    get:
      summary: HSM groups retrieval
      description: Retrieves all HSM groups.
      operationId: retrieves-all-hsm-groups
      x-api-path-slug: hsmgroups-get
      parameters:
      - in: query
        name: pageIndex
        description: If set, enables pagination and returns only the 100 HSM groups
          of the specified page
      responses:
        200:
          description: OK
      tags:
      - HSM
      - Groups
      - Retrieval