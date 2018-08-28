swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeReplicationSubnetGroups:
    get:
      summary: Describe Replication Subnet Groups
      description: Returns information about the replication subnet groups.
      operationId: describeReplicationSubnetGroups
      x-api-path-slug: actiondescribereplicationsubnetgroups-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=CreateReplicationSubnetGroup:
    get:
      summary: Create Replication Subnet Group
      description: Creates a replication subnet group given a list of the subnet IDs
        in a VPC.
      operationId: createReplicationSubnetGroup
      x-api-path-slug: actioncreatereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description for the subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name for the replication subnet group
        type: string
      - in: query
        name: SubnetIds
        description: The EC2 subnet IDs for the subnet group
        type: string
      - in: query
        name: Tags
        description: The tag to be assigned to the subnet group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
  /?Action=DeleteReplicationSubnetGroup:
    get:
      summary: Delete Replication Subnet Group
      description: Deletes a subnet group.
      operationId: deleteReplicationSubnetGroup
      x-api-path-slug: actiondeletereplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The subnet group name of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Group
  /?Action=ModifyReplicationSubnetGroup:
    get:
      summary: Modify Replication Subnet Group
      description: Modifies the settings for the specified replication subnet group.
      operationId: modifyReplicationSubnetGroup
      x-api-path-slug: actionmodifyreplicationsubnetgroup-get
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description of the replication instance subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name of the replication instance subnet group
        type: string
      - in: query
        name: SubnetIds
        description: A list of subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Subnet Groups