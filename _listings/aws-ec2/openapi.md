---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribePlacementGroups:
    get:
      summary: Describe Placement Groups
      description: Describes one or more of your placement groups.
      operationId: describeplacementgroups
      x-api-path-slug: actiondescribeplacementgroups-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: ZoneName.N
        description: The names of one or more Availability Zones
        type: string
      responses:
        200:
          description: OK
      tags:
      - Placement Groups
  /?Action=DescribeStaleSecurityGroups (EC2-VPC only):
    get:
      summary: Describe Stale Security Groups ( E C2- V P C only)
      description: '[EC2-VPC only] Describes the stale security group rules for security
        groups in a specified VPC.'
      operationId: describestalesecuritygroups-ec2vpc-only
      x-api-path-slug: actiondescribestalesecuritygroups-ec2vpc-only-get
      parameters:
      - in: query
        name: CidrIp
        description: The CIDR IP address range
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: FromPort
        description: The start of port range for the TCP and UDP protocols, or an
          ICMP type number
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: IpPermissions.N
        description: A set of IP permissions
        type: string
      - in: query
        name: IpProtocol
        description: The IP protocol name or number
        type: string
      - in: query
        name: SourceSecurityGroupName
        description: The name of a destination security group
        type: string
      - in: query
        name: SourceSecurityGroupOwnerId
        description: The AWS account number for a destination security group
        type: string
      - in: query
        name: ToPort
        description: The end of port range for the TCP and UDP protocols, or an ICMP
          type number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=RevokeSecurityGroupEgress (EC2-VPC only):
    get:
      summary: Revoke Security Group Egress ( E C2- V P C only)
      description: '[EC2-VPC only] Removes one or more egress rules from a security
        group for EC2-VPC.'
      operationId: revokesecuritygroupegress-ec2vpc-only
      x-api-path-slug: actionrevokesecuritygroupegress-ec2vpc-only-get
      parameters:
      - in: query
        name: CidrIp
        description: The CIDR IP address range
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: FromPort
        description: The start of port range for the TCP and UDP protocols, or an
          ICMP type number
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: GroupName
        description: '[EC2-Classic, default VPC] The name of the security group'
        type: string
      - in: query
        name: IpPermissions.N
        description: A set of IP permissions
        type: string
      - in: query
        name: IpProtocol
        description: The IP protocol name (tcp, udp, icmp) or number         (see
          Protocol Numbers)
        type: string
      - in: query
        name: SourceSecurityGroupName
        description: '[EC2-Classic, default VPC] The name of the source security group'
        type: string
      - in: query
        name: SourceSecurityGroupOwnerId
        description: '[EC2-Classic] The AWS account ID of the source security group,
          if the source security group is in a different account'
        type: string
      - in: query
        name: ToPort
        description: The end of port range for the TCP and UDP protocols, or an ICMP
          code number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
  /?Action=RevokeSecurityGroupIngress:
    get:
      summary: Revoke Security Group Ingress
      description: Removes one or more ingress rules from a security group.
      operationId: revokesecuritygroupingress
      x-api-path-slug: actionrevokesecuritygroupingress-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: SpotInstanceRequestId.N
        description: One or more Spot instance request IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Security Groups
---