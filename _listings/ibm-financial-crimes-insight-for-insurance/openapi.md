swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 1
info:
  title: Financial Crimes Insight for Insurance public REST APIs
  description: these-are-the-financial-crimes-insight-for-insurance-public-rest-apis-used-by-clients-to-access-the-fcii-capabilities
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/group:
    put:
      summary: Insert group data into the database
      description: This method is used to insert group data into the database.  The
        XML schema is defined in the GROUP.XSD file.
      operationId: putGroup
      x-api-path-slug: ibmfciplatformfactgroup-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Group
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/group/{id}:
    get:
      summary: Retrieve group data from the database, for the specific group id
      description: This method is used to retrieve specific group data from the database
      operationId: getGroup
      x-api-path-slug: ibmfciplatformfactgroupid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Group
      - Data
      - From
      - Database
      - The
      - Specific
      - Group
      - Id