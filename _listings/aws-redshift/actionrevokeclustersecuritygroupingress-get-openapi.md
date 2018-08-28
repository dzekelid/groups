---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Revoke Cluster Security Group Ingress
  version: 1.0.0
  description: |-
    Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                IP range or Amazon EC2 security group.
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
  /?Action=CreateClusterSecurityGroup:
    get:
      summary: Create Cluster Security Group
      description: Creates a new Amazon Redshift security group.
      operationId: createClusterSecurityGroup
      x-api-path-slug: actioncreateclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name for the security group
        type: string
      - in: query
        name: Description
        description: A description for the security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CreateClusterSubnetGroup:
    get:
      summary: Create Cluster Subnet Group
      description: Creates a new Amazon Redshift subnet group.
      operationId: createClusterSubnetGroup
      x-api-path-slug: actioncreateclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name for the subnet group
        type: string
      - in: query
        name: Description
        description: A description for the subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DeleteClusterParameterGroup:
    get:
      summary: Delete Cluster Parameter Group
      description: Deletes a specified Amazon Redshift parameter group.
      operationId: deleteClusterParameterGroup
      x-api-path-slug: actiondeleteclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteClusterSecurityGroup:
    get:
      summary: Delete Cluster Security Group
      description: Deletes an Amazon Redshift security group.
      operationId: deleteClusterSecurityGroup
      x-api-path-slug: actiondeleteclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the cluster security group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DeleteClusterSubnetGroup:
    get:
      summary: Delete Cluster Subnet Group
      description: Deletes the specified cluster subnet group.
      operationId: deleteClusterSubnetGroup
      x-api-path-slug: actiondeleteclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group name to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=ModifyClusterParameterGroup:
    get:
      summary: Modify Cluster Parameter Group
      description: Modifies the parameters of a parameter group.
      operationId: modifyClusterParameterGroup
      x-api-path-slug: actionmodifyclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be modified
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameters to be modified
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ModifyClusterSubnetGroup:
    get:
      summary: Modify Cluster Subnet Group
      description: Modifies a cluster subnet group to include the specified list of
        VPC subnets.
      operationId: modifyClusterSubnetGroup
      x-api-path-slug: actionmodifyclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group to be modified
        type: string
      - in: query
        name: Description
        description: A text description of the subnet group to be modified
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=ResetClusterParameterGroup:
    get:
      summary: Reset Cluster Parameter Group
      description: |-
        Sets one or more parameters of the specified parameter group to their default
                    values and sets the source values of the parameters to "engine-default".
      operationId: resetClusterParameterGroup
      x-api-path-slug: actionresetclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group to be reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of names of parameters to be reset
        type: string
      - in: query
        name: ResetAllParameters
        description: If true, all parameters in the specified parameter group will
          be reset            to their default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=RevokeClusterSecurityGroupIngress:
    get:
      summary: Revoke Cluster Security Group Ingress
      description: |-
        Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                    IP range or Amazon EC2 security group.
      operationId: revokeClusterSecurityGroupIngress
      x-api-path-slug: actionrevokeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range for which to revoke access
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security Group from which to revoke the ingress
          rule
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 Security Group whose access is to be revoked
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          in the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
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