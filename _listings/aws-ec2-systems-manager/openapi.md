---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePatchGroups:
    get:
      summary: Describe Patch Groups
      description: Lists all patch groups that have been registered with patch baselines.
      operationId: describePatchGroups
      x-api-path-slug: actiondescribepatchgroups-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of patch groups to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Groups
---