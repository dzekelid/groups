---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Create D B Parameter Group
  version: 1.0.0
  description: Creates a new DB parameter group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeDBSecurityGroupIngress:
    get:
      summary: Authorize D B Security Group Ingress
      description: Enables ingress to a DBSecurityGroup using one of two forms of
        authorization.
      operationId: authorizedbsecuritygroupingress
      x-api-path-slug: actionauthorizedbsecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to authorize
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to add authorization to
        type: string
      - in: query
        name: EC2SecurityGroupId
        description: Id of the EC2 security group to authorize
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: Name of the EC2 security group to authorize
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: AWS account number of the owner of the EC2 security group        specified
          in the EC2SecurityGroupName parameter
        type: string
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=CopyDBClusterParameterGroup:
    get:
      summary: Copy D B Cluster Parameter Group
      description: Copies the specified DB cluster parameter group.
      operationId: copydbclusterparametergroup
      x-api-path-slug: actioncopydbclusterparametergroup-get
      parameters:
      - in: query
        name: SourceDBClusterParameterGroupIdentifier
        description: The identifier or Amazon Resource Name (ARN) for the source DB
          cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBClusterParameterGroupDescription
        description: A description for the copied DB cluster parameter group
        type: string
      - in: query
        name: TargetDBClusterParameterGroupIdentifier
        description: The identifier for the copied DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CopyDBParameterGroup:
    get:
      summary: Copy D B Parameter Group
      description: Copies the specified DB parameter group.
      operationId: copydbparametergroup
      x-api-path-slug: actioncopydbparametergroup-get
      parameters:
      - in: query
        name: SourceDBParameterGroupIdentifier
        description: The identifier or ARN for the source DB parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetDBParameterGroupDescription
        description: A description for the copied DB parameter group
        type: string
      - in: query
        name: TargetDBParameterGroupIdentifier
        description: The identifier for the copied DB parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=CopyOptionGroup:
    get:
      summary: Copy Option Group
      description: Copies the specified option group.
      operationId: copyoptiongroup
      x-api-path-slug: actioncopyoptiongroup-get
      parameters:
      - in: query
        name: SourceOptionGroupIdentifier
        description: The identifier or ARN for the source option group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TargetOptionGroupDescription
        description: The description for the copied option group
        type: string
      - in: query
        name: TargetOptionGroupIdentifier
        description: The identifier for the copied option group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=CreateDBClusterParameterGroup:
    get:
      summary: Create D B Cluster Parameter Group
      description: Creates a new DB cluster parameter group.
      operationId: createdbclusterparametergroup
      x-api-path-slug: actioncreatedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      - in: query
        name: DBParameterGroupFamily
        description: The DB cluster parameter group family name
        type: string
      - in: query
        name: Description
        description: The description for the DB cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CreateDBParameterGroup:
    get:
      summary: Create D B Parameter Group
      description: Creates a new DB parameter group.
      operationId: createdbparametergroup
      x-api-path-slug: actioncreatedbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupFamily
        description: The DB parameter group family name
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Description
        description: The description for the DB parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
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