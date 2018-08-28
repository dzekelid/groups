---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe Option Group Options
  version: 1.0.0
  description: Describes all available options.
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
  /?Action=CreateDBSecurityGroup:
    get:
      summary: Create D B Security Group
      description: Creates a new DB security group.
      operationId: createdbsecuritygroup
      x-api-path-slug: actioncreatedbsecuritygroup-get
      parameters:
      - in: query
        name: DBSecurityGroupDescription
        description: The description for the DB security group
        type: string
      - in: query
        name: DBSecurityGroupName
        description: The name for the DB security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=CreateDBSubnetGroup:
    get:
      summary: Create D B Subnet Group
      description: Creates a new DB subnet group.
      operationId: createdbsubnetgroup
      x-api-path-slug: actioncreatedbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupDescription
        description: The description for the DB subnet group
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The name for the DB subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: The EC2 Subnet IDs for the DB subnet group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=CreateOptionGroup:
    get:
      summary: Create Option Group
      description: Creates a new option group.
      operationId: createoptiongroup
      x-api-path-slug: actioncreateoptiongroup-get
      parameters:
      - in: query
        name: EngineName
        description: Specifies the name of the engine that this option group should
          be associated with
        type: string
      - in: query
        name: MajorEngineVersion
        description: Specifies the major version of the engine that this option group
          should be associated with
        type: string
      - in: query
        name: OptionGroupDescription
        description: The description of the option group
        type: string
      - in: query
        name: OptionGroupName
        description: Specifies the name of the option group to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DeleteDBClusterParameterGroup:
    get:
      summary: Delete D B Cluster Parameter Group
      description: Deletes a specified DB cluster parameter group.
      operationId: deletedbclusterparametergroup
      x-api-path-slug: actiondeletedbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteDBParameterGroup:
    get:
      summary: Delete D B Parameter Group
      description: Deletes a specified DBParameterGroup.
      operationId: deletedbparametergroup
      x-api-path-slug: actiondeletedbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
  /?Action=DeleteDBSecurityGroup:
    get:
      summary: Delete D B Security Group
      description: Deletes a DB security group.
      operationId: deletedbsecuritygroup
      x-api-path-slug: actiondeletedbsecuritygroup-get
      parameters:
      - in: query
        name: DBSecurityGroupName
        description: The name of the DB security group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=DeleteDBSubnetGroup:
    get:
      summary: Delete D B Subnet Group
      description: Deletes a DB subnet group.
      operationId: deletedbsubnetgroup
      x-api-path-slug: actiondeletedbsubnetgroup-get
      parameters:
      - in: query
        name: DBSubnetGroupName
        description: The name of the database subnet group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet Groups
  /?Action=DeleteOptionGroup:
    get:
      summary: Delete Option Group
      description: Deletes an existing option group.
      operationId: deleteoptiongroup
      x-api-path-slug: actiondeleteoptiongroup-get
      parameters:
      - in: query
        name: OptionGroupName
        description: The name of the option group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
  /?Action=DescribeOptionGroupOptions:
    get:
      summary: Describe Option Group Options
      description: Describes all available options.
      operationId: describeoptiongroupoptions
      x-api-path-slug: actiondescribeoptiongroupoptions-get
      parameters:
      - in: query
        name: EngineName
        description: A required parameter
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: MajorEngineVersion
        description: If specified, filters the results to include only options for
          the specified major engine version
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Option Groups
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