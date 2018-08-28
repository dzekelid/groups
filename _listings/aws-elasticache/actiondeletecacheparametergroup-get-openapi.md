---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Delete Cache Parameter Group
  version: 1.0.0
  description: |-
    Deletes the specified cache parameter
                group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCacheParameterGroups:
    get:
      summary: Describe Cache Parameter Groups
      description: |-
        Returns a list of cache parameter group
                    descriptions.
      operationId: describeCacheParameterGroups
      x-api-path-slug: actiondescribecacheparametergroups-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of a specific cache parameter group to return details
          for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=DescribeCacheSecurityGroups:
    get:
      summary: Describe Cache Security Groups
      description: |-
        Returns a list of cache security group
                    descriptions.
      operationId: describeCacheSecurityGroups
      x-api-path-slug: actiondescribecachesecuritygroups-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The name of the cache security group to return details for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=DescribeCacheSubnetGroups:
    get:
      summary: Describe Cache Subnet Groups
      description: |-
        Returns a list of cache subnet group
                    descriptions.
      operationId: describeCacheSubnetGroups
      x-api-path-slug: actiondescribecachesubnetgroups-get
      parameters:
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to return details for
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=DescribeReplicationGroups:
    get:
      summary: Describe Replication Groups
      description: |-
        Returns information about a particular
                    replication group.
      operationId: describeReplicationGroups
      x-api-path-slug: actiondescribereplicationgroups-get
      parameters:
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier for the replication group to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Groups
  /?Action=AuthorizeCacheSecurityGroupIngress:
    get:
      summary: Authorize Cache Security Group Ingress
      description: |-
        Allows network ingress to a cache
                    security group.
      operationId: authorizeCacheSecurityGroupIngress
      x-api-path-slug: actionauthorizecachesecuritygroupingress-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The cache security group that allows network ingress
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The Amazon EC2 security group to be authorized for ingress to
          the cache security group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the Amazon EC2 security group owner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=CreateCacheParameterGroup:
    get:
      summary: Create Cache Parameter Group
      description: Creates a new cache parameter group.
      operationId: createCacheParameterGroup
      x-api-path-slug: actioncreatecacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of the cache parameter group family that the cache parameter
          group can be used with
        type: string
      - in: query
        name: CacheParameterGroupName
        description: A user-specified name for the cache parameter group
        type: string
      - in: query
        name: Description
        description: A user-specified description for the cache parameter group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
  /?Action=CreateCacheSecurityGroup:
    get:
      summary: Create Cache Security Group
      description: Creates a new cache security group.
      operationId: createCacheSecurityGroup
      x-api-path-slug: actioncreatecachesecuritygroup-get
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: A name for the cache security group
        type: string
      - in: query
        name: Description
        description: A description for the cache security group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Security Groups
  /?Action=CreateCacheSubnetGroup:
    get:
      summary: Create Cache Subnet Group
      description: Creates a new cache subnet group.
      operationId: createCacheSubnetGroup
      x-api-path-slug: actioncreatecachesubnetgroup-get
      parameters:
      - in: query
        name: CacheSubnetGroupDescription
        description: A description for the cache subnet group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: A name for the cache subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: A list of VPC subnet IDs for the cache subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Subnet Groups
  /?Action=CreateReplicationGroup:
    get:
      summary: Create Replication Group
      description: Creates a Redis (cluster mode disabled) or a Redis (cluster mode
        enabled) replication group.
      operationId: createReplicationGroup
      x-api-path-slug: actioncreatereplicationgroup-get
      parameters:
      - in: query
        name: AuthToken
        description: Reserved parameter
        type: string
      - in: query
        name: AutomaticFailoverEnabled
        description: Specifies whether a read-only replica is automatically promoted
          to read/write primary if the existing primary fails
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: This parameter is currently disabled
        type: string
      - in: query
        name: CacheNodeType
        description: The compute and memory capacity of the nodes in the node group
          (shard)
        type: string
      - in: query
        name: CacheParameterGroupName
        description: The name of the parameter group to associate with this replication
          group
        type: string
      - in: query
        name: CacheSecurityGroupNames.CacheSecurityGroupName.N
        description: A list of cache security group names to associate with this replication
          group
        type: string
      - in: query
        name: CacheSubnetGroupName
        description: The name of the cache subnet group to be used for the replication
          group
        type: string
      - in: query
        name: Engine
        description: The name of the cache engine to be used for the cache clusters
          in this replication group
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the cache engine to be used for the cache
          clusters in this replication group
        type: string
      - in: query
        name: NodeGroupConfiguration.NodeGroupConfiguration.N
        description: A list of node group (shard) configuration options
        type: string
      - in: query
        name: NotificationTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon Simple Notification
          Service (SNS) topic to which notifications are sent
        type: string
      - in: query
        name: NumCacheClusters
        description: The number of clusters this replication group initially has
        type: string
      - in: query
        name: NumNodeGroups
        description: An optional parameter that specifies the number of node groups
          (shards) for this Redis (cluster mode enabled) replication group
        type: string
      - in: query
        name: Port
        description: The port number on which each member of the replication group
          accepts connections
        type: string
      - in: query
        name: PreferredCacheClusterAZs.AvailabilityZone.N
        description: A list of EC2 Availability Zones in which the replication groups
          cache clusters are created
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: Specifies the weekly time range during which maintenance    on
          the cache cluster is performed
        type: string
      - in: query
        name: PrimaryClusterId
        description: The identifier of the cache cluster that serves as the primary
          for this replication            group
        type: string
      - in: query
        name: ReplicasPerNodeGroup
        description: An optional parameter that specifies the number of replica nodes
          in each node group (shard)
        type: string
      - in: query
        name: ReplicationGroupDescription
        description: A user-created description for the replication group
        type: string
      - in: query
        name: ReplicationGroupId
        description: The replication group identifier
        type: string
      - in: query
        name: SecurityGroupIds.SecurityGroupId.N
        description: One or more Amazon VPC security groups associated with this replication
          group
        type: string
      - in: query
        name: SnapshotArns.SnapshotArn.N
        description: A list of Amazon Resource Names (ARN) that uniquely identify           the
          Redis RDB snapshot files stored in Amazon S3
        type: string
      - in: query
        name: SnapshotName
        description: The name of a snapshot from which to restore data into the new
          replication group
        type: string
      - in: query
        name: SnapshotRetentionLimit
        description: The number of days for which ElastiCache retains automatic snapshots
          before deleting them
        type: string
      - in: query
        name: SnapshotWindow
        description: The daily time range (in UTC) during which ElastiCache begins
          taking a daily snapshot of your node group (shard)
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of cost allocation tags to be added to this resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Groups
  /?Action=DeleteCacheParameterGroup:
    get:
      summary: Delete Cache Parameter Group
      description: |-
        Deletes the specified cache parameter
                    group.
      operationId: deleteCacheParameterGroup
      x-api-path-slug: actiondeletecacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
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