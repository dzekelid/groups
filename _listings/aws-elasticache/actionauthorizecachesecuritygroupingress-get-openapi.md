---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Authorize Cache Security Group Ingress
  version: 1.0.0
  description: |-
    Allows network ingress to a cache
                security group.
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