swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachLoadBalancerTargetGroups:
    get:
      summary: Attach Load Balancer Target Groups
      description: Attaches one or more target groups to the specified Auto Scaling
        group.
      operationId: attachLoadBalancerTargetGroups
      x-api-path-slug: actionattachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeAutoScalingGroups:
    get:
      summary: Describe Auto Scaling Groups
      description: Describes one or more Auto Scaling groups.
      operationId: describeAutoScalingGroups
      x-api-path-slug: actiondescribeautoscalinggroups-get
      parameters:
      - in: query
        name: AutoScalingGroupNames.member.N
        description: The group names
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=DescribeLoadBalancerTargetGroups:
    get:
      summary: Describe Load Balancer Target Groups
      description: Describes the target groups for the specified Auto Scaling group.
      operationId: describeLoadBalancerTargetGroups
      x-api-path-slug: actiondescribeloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DetachLoadBalancerTargetGroups:
    get:
      summary: Detach Load Balancer Target Groups
      description: Detaches one or more target groups from the specified Auto Scaling
        group.
      operationId: detachLoadBalancerTargetGroups
      x-api-path-slug: actiondetachloadbalancertargetgroups-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=CreateAutoScalingGroup:
    get:
      summary: Create Auto Scaling Group
      description: Creates an Auto Scaling group with the specified name and attributes.
      operationId: createAutoScalingGroup
      x-api-path-slug: actioncreateautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: AvailabilityZones.member.N
        description: One or more Availability Zones for the group
        type: string
      - in: query
        name: DefaultCooldown
        description: The amount of time, in seconds, after a scaling activity completes
          before another scaling activity can start
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: HealthCheckGracePeriod
        description: The amount of time, in seconds, that Auto Scaling waits before
          checking the health status of an EC2 instance that has come into service
        type: string
      - in: query
        name: HealthCheckType
        description: The service to use for the health checks
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance used to create a launch configuration
          for the group
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: LoadBalancerNames.member.N
        description: One or more Classic load balancers
        type: string
      - in: query
        name: MaxSize
        description: The maximum size of the group
        type: string
      - in: query
        name: MinSize
        description: The minimum size of the group
        type: string
      - in: query
        name: NewInstancesProtectedFromScaleIn
        description: Indicates whether newly launched instances are protected from
          termination by Auto Scaling when scaling in
        type: string
      - in: query
        name: PlacementGroup
        description: The name of the placement group into which youll launch your
          instances, if any
        type: string
      - in: query
        name: Tags.member.N
        description: One or more tags
        type: string
      - in: query
        name: TargetGroupARNs.member.N
        description: The Amazon Resource Names (ARN) of the target groups
        type: string
      - in: query
        name: TerminationPolicies.member.N
        description: One or more termination policies used to select the instance
          to terminate
        type: string
      - in: query
        name: VPCZoneIdentifier
        description: A comma-separated list of subnet identifiers for your virtual
          private cloud (VPC)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=DeleteAutoScalingGroup:
    get:
      summary: Delete Auto Scaling Group
      description: Deletes the specified Auto Scaling group.
      operationId: deleteAutoScalingGroup
      x-api-path-slug: actiondeleteautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group to delete
        type: string
      - in: query
        name: ForceDelete
        description: Specifies that the group will be deleted along with all instances
          associated with the group, without waiting for all instances to be terminated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Groups
  /?Action=PutLifecycleHook:
    get:
      summary: Put Lifecycle Hook
      description: Creates or updates a lifecycle hook for the specified Auto Scaling
        Group.
      operationId: putLifecycleHook
      x-api-path-slug: actionputlifecyclehook-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group to which you want to assign
          the lifecycle hook
        type: string
      - in: query
        name: DefaultResult
        description: Defines the action the Auto Scaling group should take when the
          lifecycle hook timeout elapses or if an unexpected failure occurs
        type: string
      - in: query
        name: HeartbeatTimeout
        description: The amount of time, in seconds, that can elapse before the lifecycle
          hook times out
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      - in: query
        name: LifecycleTransition
        description: The instance state to which you want to attach the lifecycle
          hook
        type: string
      - in: query
        name: NotificationMetadata
        description: Contains additional information that you want to include any
          time Auto Scaling sends a message to the notification target
        type: string
      - in: query
        name: NotificationTargetARN
        description: The ARN of the notification target that Auto Scaling will use
          to notify you when an instance is in the transition state for the lifecycle
          hook
        type: string
      - in: query
        name: RoleARN
        description: The ARN of the IAM role that allows the Auto Scaling group to
          publish to the specified notification target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=PutScheduledUpdateGroupAction:
    get:
      summary: Put Scheduled Update Group Action
      description: Creates or updates a scheduled scaling action for an Auto Scaling
        group.
      operationId: putScheduledUpdateGroupAction
      x-api-path-slug: actionputscheduledupdategroupaction-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the group
        type: string
      - in: query
        name: EndTime
        description: The time for the recurring schedule to end
        type: string
      - in: query
        name: MaxSize
        description: The maximum size for the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size for the Auto Scaling group
        type: string
      - in: query
        name: Recurrence
        description: The recurring schedule for this action, in Unix cron syntax format
        type: string
      - in: query
        name: ScheduledActionName
        description: The name of this scaling action
        type: string
      - in: query
        name: StartTime
        description: The time for this action to start, in YYYY-MM-DDThh:mm:ssZ format
          in UTC/GMT only             (for example, 2014-06-01T00:00:00Z)
        type: string
      - in: query
        name: Time
        description: This parameter is deprecated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Update
  /?Action=TerminateInstanceInAutoScalingGroup:
    get:
      summary: Terminate Instance In Auto Scaling Group
      description: Terminates the specified instance and optionally adjusts the desired
        group size.
      operationId: terminateInstanceInAutoScalingGroup
      x-api-path-slug: actionterminateinstanceinautoscalinggroup-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If true, terminating the instance also decrements the size of
          the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Auto Scaling
  /?Action=UpdateAutoScalingGroup:
    get:
      summary: Update Auto Scaling Group
      description: Updates the configuration for the specified Auto Scaling group.
      operationId: updateAutoScalingGroup
      x-api-path-slug: actionupdateautoscalinggroup-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: AvailabilityZones.member.N
        description: One or more Availability Zones for the group
        type: string
      - in: query
        name: DefaultCooldown
        description: The amount of time, in seconds, after a scaling activity completes
          before another scaling activity can start
        type: string
      - in: query
        name: DesiredCapacity
        description: The number of EC2 instances that should be running in the Auto
          Scaling group
        type: string
      - in: query
        name: HealthCheckGracePeriod
        description: The amount of time, in seconds, that Auto Scaling waits before
          checking the health status of an EC2 instance that has come into service
        type: string
      - in: query
        name: HealthCheckType
        description: The service to use for the health checks
        type: string
      - in: query
        name: LaunchConfigurationName
        description: The name of the launch configuration
        type: string
      - in: query
        name: MaxSize
        description: The maximum size of the Auto Scaling group
        type: string
      - in: query
        name: MinSize
        description: The minimum size of the Auto Scaling group
        type: string
      - in: query
        name: NewInstancesProtectedFromScaleIn
        description: Indicates whether newly launched instances are protected from
          termination by Auto Scaling when scaling in
        type: string
      - in: query
        name: PlacementGroup
        description: The name of the placement group into which youll launch your
          instances, if any
        type: string
      - in: query
        name: TerminationPolicies.member.N
        description: A standalone termination policy or a list of termination policies
          used to select the instance to terminate
        type: string
      - in: query
        name: VPCZoneIdentifier
        description: The ID of the subnet, if you are launching into a VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling