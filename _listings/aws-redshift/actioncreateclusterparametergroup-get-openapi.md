---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Create Cluster Parameter Group
  version: 1.0.0
  description: Creates an Amazon Redshift parameter group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeClusterParameterGroups:
    get:
      summary: Describe Cluster Parameter Groups
      description: |-
        Returns a list of Amazon Redshift parameter groups, including parameter groups you
                    created and the default parameter group.
      operationId: describeClusterParameterGroups
      x-api-path-slug: actiondescribeclusterparametergroups-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a specific parameter group for which to return details
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          parameter            groups that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster parameter            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeClusterSecurityGroups:
    get:
      summary: Describe Cluster Security Groups
      description: Returns information about Amazon Redshift security groups.
      operationId: describeClusterSecurityGroups
      x-api-path-slug: actiondescribeclustersecuritygroups-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of a cluster security group for which you are requesting
          details
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          security groups            that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster security            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DescribeClusterSubnetGroups:
    get:
      summary: Describe Cluster Subnet Groups
      description: |-
        Returns one or more cluster subnet group objects, which contain metadata about your
                    cluster subnet groups.
      operationId: describeClusterSubnetGroups
      x-api-path-slug: actiondescribeclustersubnetgroups-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group for which information is
          requested
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          subnet groups            that are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster subnet            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=AuthorizeClusterSecurityGroupIngress:
    get:
      summary: Authorize Cluster Security Group Ingress
      description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
      operationId: authorizeClusterSecurityGroupIngress
      x-api-path-slug: actionauthorizeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to be added the Amazon Redshift security group
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security group to which the ingress rule is added
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The EC2 security group to be added the Amazon Redshift security
          group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          by the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CreateClusterParameterGroup:
    get:
      summary: Create Cluster Parameter Group
      description: Creates an Amazon Redshift parameter group.
      operationId: createClusterParameterGroup
      x-api-path-slug: actioncreateclusterparametergroup-get
      parameters:
      - in: query
        name: Description
        description: A description of the parameter group
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The Amazon Redshift engine version to which the cluster parameter
          group applies
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
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