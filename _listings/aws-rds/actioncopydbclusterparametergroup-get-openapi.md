---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Copy D B Cluster Parameter Group
  version: 1.0.0
  description: Copies the specified DB cluster parameter group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDBClusterParameterGroups:
    get:
      summary: Describe D B Cluster Parameter Groups
      description: Returns a list of DBClusterParameterGroup descriptions.
      operationId: describedbclusterparametergroups
      x-api-path-slug: actiondescribedbclusterparametergroups-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of a specific DB cluster parameter group to return details
          for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBClusterParameterGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeDBParameterGroups:
    get:
      summary: Describe D B Parameter Groups
      description: Returns a list of DBParameterGroup descriptions.
      operationId: describedbparametergroups
      x-api-path-slug: actiondescribedbparametergroups-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of a specific DB parameter group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBParameterGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=DescribeDBSecurityGroups:
    get:
      summary: Describe D B Security Groups
      description: Returns a list of DBSecurityGroup descriptions.
      operationId: describedbsecuritygroups
      x-api-path-slug: actiondescribedbsecuritygroups-get
      parameters:
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBSecurityGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=DescribeDBSubnetGroups:
    get:
      summary: Describe D B Subnet Groups
      description: Returns a list of DBSubnetGroup descriptions.
      operationId: describedbsubnetgroups
      x-api-path-slug: actiondescribedbsubnetgroups-get
      parameters:
      - in: query
        name: DBSubnetGroupName
        description: The name of the DB subnet group to return details for
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeDBSubnetGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=DescribeOptionGroups:
    get:
      summary: Describe Option Groups
      description: Describes the available option groups.
      operationId: describeoptiongroups
      x-api-path-slug: actiondescribeoptiongroups-get
      parameters:
      - in: query
        name: EngineName
        description: Filters the list of option groups to only include groups associated
          with a specific database engine
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: MajorEngineVersion
        description: Filters the list of option groups to only include groups associated
          with a specific database engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous DescribeOptionGroups
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=RevokeDBSecurityGroupIngress:
    get:
      summary: Revoke D B Security Group Ingress
      description: Revokes ingress from a DBSecurityGroup for previously authorized
        IP ranges or EC2 or VPC Security Groups.
      operationId: revokedbsecuritygroupingress
      x-api-path-slug: actionrevokedbsecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to revoke access from
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to revoke ingress from
        type: string
      - in: query
        name: EC2SecurityGroupId
        description: The id of the EC2 security group to revoke access from
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 security group to revoke access from
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS Account Number of the owner of the EC2 security group        specified
          in the EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
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