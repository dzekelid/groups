{
  "info": {
    "name": "AWS Auto Scaling API Put Scheduled Update Group Action",
    "_postman_id": "e3d635cc-01b3-4794-8de0-081615e749dc",
    "description": "Creates or updates a scheduled scaling action for an Auto Scaling group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Server Instance",
      "item": [
        {
          "id": "d8ef24b2-f3e4-4e31-a6ec-bea2777ba8e8",
          "name": "attachInstances",
          "request": {
            "url": "http://example.com/api/?Action=AttachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more EC2 instances to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e91e629-fe27-439a-996f-774a4b987f48"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "22c1d4f6-16a6-4f88-a06d-0a72a35cdc37",
          "name": "attachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more Classic load balancers to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58a3fe18-428d-42f6-86d4-99fa94c03143"
            }
          ]
        },
        {
          "id": "48961df0-6481-4487-b302-c4507e7acc54",
          "name": "attachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more target groups to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d3c59e0-5412-496b-a09a-5d594472f0bc"
            }
          ]
        },
        {
          "id": "d5d669c6-96c2-4f04-866d-cc68f2d6feeb",
          "name": "describeLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the load balancers for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "152106e1-f9ae-46a5-b418-55e58a4f8354"
            }
          ]
        },
        {
          "id": "5f8e9eb0-d260-4fdb-8987-a31fedce1761",
          "name": "describeLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the target groups for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0123cf87-5be1-4bd6-83e0-968cae41097d"
            }
          ]
        },
        {
          "id": "efde788f-c42e-43ec-a8e6-9e353436f576",
          "name": "detachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more Classic load balancers from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "390c7b2d-65c0-413f-a0ab-58c03170af30"
            }
          ]
        },
        {
          "id": "023dd7be-0f9e-47d3-a128-b29686b90aa8",
          "name": "detachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more target groups from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41b14f32-1372-4b9d-ae2b-5d8f664b3fee"
            }
          ]
        }
      ]
    },
    {
      "name": "Life Cycle",
      "item": [
        {
          "id": "8572b5d4-1654-4d0a-953b-d47898296532",
          "name": "completeLifecycleAction",
          "request": {
            "url": "http://example.com/api/?Action=CompleteLifecycleAction?AutoScalingGroupName=AutoScalingGroupName&InstanceId=InstanceId&LifecycleActionResult=LifecycleActionResult&LifecycleActionToken=LifecycleActionToken&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Completes the lifecycle action for the specified token or instance with the specified result."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "294ec367-fa21-4328-9c82-3d77881af7de"
            }
          ]
        },
        {
          "id": "00aee21a-df6d-4bc5-b9b2-3bc31eefdf63",
          "name": "deleteLifecycleHook",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLifecycleHook?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified lifecycle hook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c730d65e-70cc-4b07-b959-b29281158307"
            }
          ]
        },
        {
          "id": "408e7fc7-5a11-443c-825f-6643a356faac",
          "name": "describeLifecycleHooks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHooks?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookNames.member.N=LifecycleHookNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the lifecycle hooks for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "68b63342-74c6-43eb-84e8-8a287d507eed"
            }
          ]
        },
        {
          "id": "46e08ff4-2ef4-4311-b6eb-3580807dbb38",
          "name": "describeLifecycleHookTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHookTypes?LifecycleHookTypes.member.N=LifecycleHookTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available types of lifecycle hooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beb6eb51-1f43-4b47-8e41-2b29f97805ec"
            }
          ]
        },
        {
          "id": "d03ed8f9-26a3-48e2-b66b-954283e8526f",
          "name": "putLifecycleHook",
          "request": {
            "url": "http://example.com/api/?Action=PutLifecycleHook?AutoScalingGroupName=AutoScalingGroupName&DefaultResult=DefaultResult&HeartbeatTimeout=HeartbeatTimeout&LifecycleHookName=LifecycleHookName&LifecycleTransition=LifecycleTransition&NotificationMetadata=NotificationMetadata&NotificationTargetARN=NotificationTargetARN&RoleARN=RoleARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a lifecycle hook for the specified Auto Scaling Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd4ffe97-1d69-465d-8d6a-1ab1581568de"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Groups",
      "item": [
        {
          "id": "ab0f9419-7080-4c17-91f2-56c3c118f40e",
          "name": "createAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&AvailabilityZones.member.N=AvailabilityZones.member.N&DefaultCooldown=DefaultCooldown&DesiredCapacity=DesiredCapacity&HealthCheckGracePeriod=HealthCheckGracePeriod&HealthCheckType=HealthCheckType&InstanceId=InstanceId&LaunchConfigurationName=LaunchConfigurationName&LoadBalancerNames.member.N=LoadBalancerNames.member.N&MaxSize=MaxSize&MinSize=MinSize&NewInstancesProtectedFromScaleIn=NewInstancesProtectedFromScaleIn&PlacementGroup=PlacementGroup&Tags.member.N=Tags.member.N&TargetGroupARNs.member.N=TargetGroupARNs.member.N&TerminationPolicies.member.N=TerminationPolicies.member.N&VPCZoneIdentifier=VPCZoneIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Auto Scaling group with the specified name and attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f6a7b2c-678b-4c38-9401-74cd0e420156"
            }
          ]
        },
        {
          "id": "edc94be0-f348-4e69-b15a-7db0a42de98b",
          "name": "deleteAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&ForceDelete=ForceDelete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "961946f4-0c95-4f3f-b890-a9040486da38"
            }
          ]
        },
        {
          "id": "bfdaa339-95a6-4d4d-bdd4-3b2e4a2d5fde",
          "name": "describeAutoScalingGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingGroups?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "592130d3-9e9d-4b39-a089-aa80bb655026"
            }
          ]
        }
      ]
    },
    {
      "name": "Launch",
      "item": [
        {
          "id": "d043fe25-dfaf-4d21-bd71-15fd4442c911",
          "name": "createLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateLaunchConfiguration?AssociatePublicIpAddress=AssociatePublicIpAddress&BlockDeviceMappings.member.N=BlockDeviceMappings.member.N&ClassicLinkVPCId=ClassicLinkVPCId&ClassicLinkVPCSecurityGroups.member.N=ClassicLinkVPCSecurityGroups.member.N&EbsOptimized=EbsOptimized&IamInstanceProfile=IamInstanceProfile&ImageId=ImageId&InstanceId=InstanceId&InstanceMonitoring=InstanceMonitoring&InstanceType=InstanceType&KernelId=KernelId&KeyName=KeyName&LaunchConfigurationName=LaunchConfigurationName&PlacementTenancy=PlacementTenancy&RamdiskId=RamdiskId&SecurityGroups.member.N=SecurityGroups.member.N&SpotPrice=SpotPrice&UserData=UserData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ce8ab45-7e7b-435b-9639-2e0a071c0890"
            }
          ]
        },
        {
          "id": "d9c3c634-020f-467a-9527-61f4c5eecf8b",
          "name": "deleteLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLaunchConfiguration?LaunchConfigurationName=LaunchConfigurationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f04d19b6-ff31-4aa6-8c00-1bb2fb10208f"
            }
          ]
        },
        {
          "id": "0bd694c8-3e8f-479a-955e-653ce48a3087",
          "name": "describeLaunchConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLaunchConfigurations?LaunchConfigurationNames.member.N=LaunchConfigurationNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more launch configurations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c0c7d1e-d1b5-4863-901c-b63e697d1688"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "cd041671-d3c0-49c8-afbe-72ed657a5cc8",
          "name": "createOrUpdateTags",
          "request": {
            "url": "http://example.com/api/?Action=CreateOrUpdateTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates tags for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d31e721-4e06-4b8d-877c-03b4f9311dac"
            }
          ]
        },
        {
          "id": "17dbdff2-dcfc-4c63-b2d4-92f1b6ecc35e",
          "name": "deleteTags",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4047941f-aece-4d1c-a6b0-386b8546fcdf"
            }
          ]
        },
        {
          "id": "93a68cf3-7059-491b-8d9c-e5b52091a226",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?Filters.member.N=Filters.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a375c85c-2ac9-4602-ac72-41bce8d009ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Notifications",
      "item": [
        {
          "id": "90dc5429-761b-44af-9b37-71acae9753b8",
          "name": "deleteNotificationConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteNotificationConfiguration?AutoScalingGroupName=AutoScalingGroupName&TopicARN=TopicARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified notification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "896f9b8a-5599-4236-a332-09e7de823ea6"
            }
          ]
        },
        {
          "id": "fbdee0b6-8866-4f4d-a2da-bded522f8510",
          "name": "describeNotificationConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeNotificationConfigurations?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification actions associated with the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bc98235-9e38-4900-bab4-3a0201dd7da6"
            }
          ]
        },
        {
          "id": "46bc8fc5-b24e-45a9-8ecf-6cc95d13c89f",
          "name": "putNotificationConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=PutNotificationConfiguration?AutoScalingGroupName=AutoScalingGroupName&NotificationTypes.member.N=NotificationTypes.member.N&TopicARN=TopicARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an Auto Scaling group to send notifications when specified events take place."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d59d9ee5-f605-43c4-92eb-7177ee4807ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "5b10360e-3724-4a87-948d-c1fd9f5a2925",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?AutoScalingGroupName=AutoScalingGroupName&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b641fce-fb50-4d40-9b5d-a2cf1d95e1ba"
            }
          ]
        },
        {
          "id": "54d4dd2f-fcaa-4e45-b230-d36823fb583b",
          "name": "describePolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribePolicies?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken&PolicyNames.member.N=PolicyNames.member.N&PolicyTypes.member.N=PolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policies for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "160d8a0e-843b-44fc-b070-65f47e8be7c8"
            }
          ]
        },
        {
          "id": "c4629295-02b5-47ef-b2ba-1865fcd9b927",
          "name": "executePolicy",
          "request": {
            "url": "http://example.com/api/?Action=ExecutePolicy?AutoScalingGroupName=AutoScalingGroupName&BreachThreshold=BreachThreshold&HonorCooldown=HonorCooldown&MetricValue=MetricValue&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95c6833c-8944-4c1e-832e-f85eb7644321"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Action",
      "item": [
        {
          "id": "3350a999-b76b-42a0-bb44-ccf9609b234a",
          "name": "deleteScheduledAction",
          "request": {
            "url": "http://example.com/api/?Action=DeleteScheduledAction?AutoScalingGroupName=AutoScalingGroupName&ScheduledActionName=ScheduledActionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified scheduled action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b20cc115-ec2d-43bd-a7f4-b4fb139590ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "da17f2e4-65d6-40e0-913d-46329a7457d6",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?MaxNumberOfAutoScalingGroups=MaxNumberOfAutoScalingGroups&MaxNumberOfLaunchConfigurations=MaxNumberOfLaunchConfigurations&NumberOfAutoScalingGroups=NumberOfAutoScalingGroups&NumberOfLaunchConfigurations=NumberOfLaunchConfigurations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the current Auto Scaling resource limits for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0dda546f-ea70-43f4-b85d-49312fb2dc56"
            }
          ]
        }
      ]
    },
    {
      "name": "Adjustment Types",
      "item": [
        {
          "id": "847916cd-4c9f-4ae3-81a3-1559c926011a",
          "name": "describeAdjustmentTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAdjustmentTypes?AdjustmentTypes.member.N=AdjustmentTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policy adjustment types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "941f42fd-e07b-4e5a-97e0-fd02527bd463"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Instances",
      "item": [
        {
          "id": "1ffae9ee-eb9e-4cda-8a33-02efa1426b1f",
          "name": "describeAutoScalingInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingInstances?InstanceIds.member.N=InstanceIds.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27b54737-7aec-4744-8ae7-199ab65ba644"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Notifications",
      "item": [
        {
          "id": "ee9c92a9-8006-436d-8286-4f0d418e30d5",
          "name": "describeAutoScalingNotificationTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingNotificationTypes?AutoScalingNotificationTypes.member.N=AutoScalingNotificationTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification types that are supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a649a849-a520-42e6-ab6b-0fc2ccf7e07a"
            }
          ]
        }
      ]
    },
    {
      "name": "Metric Collection",
      "item": [
        {
          "id": "2be092b7-933e-45ca-a31d-edb0560034dc",
          "name": "describeMetricCollectionTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMetricCollectionTypes?Granularities.member.N=Granularities.member.N&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available CloudWatch metrics for Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "112dae40-2d49-4eea-8112-3662a159e9b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Activities",
      "item": [
        {
          "id": "86847c89-a553-4166-9ebf-ca35c025ca39",
          "name": "describeScalingActivities",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingActivities?ActivityIds.member.N=ActivityIds.member.N&AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more scaling activities for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62c27e13-b592-4677-aa56-8dec079527b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Process",
      "item": [
        {
          "id": "bdeb5093-8432-4da7-89a4-42a9a6452545",
          "name": "describeScalingProcessTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingProcessTypes?Processes.member.N=Processes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the scaling process types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a255ec73-e798-49bc-8cb6-82feffb89df9"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Actions",
      "item": [
        {
          "id": "1d823baf-7ad4-47ff-a1f7-f8d953d7c736",
          "name": "describeScheduledActions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScheduledActions?AutoScalingGroupName=AutoScalingGroupName&EndTime=EndTime&MaxRecords=MaxRecords&NextToken=NextToken&ScheduledActionNames.member.N=ScheduledActionNames.member.N&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the actions scheduled for your Auto Scaling group that haven't run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7967f9c6-3971-41f1-813f-1563c2e3414d"
            }
          ]
        }
      ]
    },
    {
      "name": "Termination Policies",
      "item": [
        {
          "id": "55dc0d70-8731-4483-a8eb-143ad2ec5b86",
          "name": "describeTerminationPolicyTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTerminationPolicyTypes?TerminationPolicyTypes.member.N=TerminationPolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the termination policies supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58425400-8bfb-43cc-9361-f5570a7a124a"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Instances",
      "item": [
        {
          "id": "5248cbc0-4965-47ba-8937-09208139c254",
          "name": "detachInstances",
          "request": {
            "url": "http://example.com/api/?Action=DetachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes one or more instances from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ff46402-0fb3-4717-8cdc-fc3fc0d12956"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics Collection",
      "item": [
        {
          "id": "3bd198a7-3cb2-4d95-a1a2-3cb21af8c12a",
          "name": "disableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=DisableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06d43091-78c7-4224-a471-447cf4a5ffd2"
            }
          ]
        },
        {
          "id": "dc0b17d0-8f70-46d5-9a66-3cf10d7954e4",
          "name": "enableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=EnableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Granularity=Granularity&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56935ed7-765d-4c68-bac4-148c05534678"
            }
          ]
        }
      ]
    },
    {
      "name": "Stand By",
      "item": [
        {
          "id": "9d40ee8f-3af8-4e3b-8ad3-a0fc3aa93920",
          "name": "enterStandby",
          "request": {
            "url": "http://example.com/api/?Action=EnterStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances into Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb0633ce-fdcf-4c88-b1aa-225db988a26f"
            }
          ]
        },
        {
          "id": "a6150bc5-3696-412d-8ebb-65a461e9e344",
          "name": "exitStandby",
          "request": {
            "url": "http://example.com/api/?Action=ExitStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances out of Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cb60caf-055f-42af-bff7-45acb9db0ab2"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Policy",
      "item": [
        {
          "id": "a4595f8e-17f5-4b27-b8be-d9c2d54729ed",
          "name": "putScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutScalingPolicy?AdjustmentType=AdjustmentType&AutoScalingGroupName=AutoScalingGroupName&Cooldown=Cooldown&EstimatedInstanceWarmup=EstimatedInstanceWarmup&MetricAggregationType=MetricAggregationType&MinAdjustmentMagnitude=MinAdjustmentMagnitude&MinAdjustmentStep=MinAdjustmentStep&PolicyName=PolicyName&PolicyType=PolicyType&ScalingAdjustment=ScalingAdjustment&StepAdjustments.member.N=StepAdjustments.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a policy for an Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2fa617a-4bfc-46d1-9633-9ea146149e6a"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Update",
      "item": [
        {
          "id": "9f5fe36a-ac7c-4604-bf58-e6c3f4fa2d72",
          "name": "putScheduledUpdateGroupAction",
          "request": {
            "url": "http://example.com/api/?Action=PutScheduledUpdateGroupAction?AutoScalingGroupName=AutoScalingGroupName&DesiredCapacity=DesiredCapacity&EndTime=EndTime&MaxSize=MaxSize&MinSize=MinSize&Recurrence=Recurrence&ScheduledActionName=ScheduledActionName&StartTime=StartTime&Time=Time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a scheduled scaling action for an Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f838338-3f1c-4bfd-9337-db3d8a956e7c"
            }
          ]
        }
      ]
    }
  ]
}