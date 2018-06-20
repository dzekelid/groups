---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Get Deployment Group
  version: 1.0.0
  description: Gets information about a deployment group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BatchGetDeploymentGroups:
    get:
      summary: Batch Get Deployment Groups
      description: Gets information about one or more deployment groups.
      operationId: batchGetDeploymentGroups
      x-api-path-slug: actionbatchgetdeploymentgroups-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupNames
        description: The deployment groups names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=CreateDeploymentGroup:
    get:
      summary: Create Deployment Group
      description: |-
        Creates a deployment group to which application revisions will be
                    deployed.
      operationId: createDeploymentGroup
      x-api-path-slug: actioncreatedeploymentgroup-get
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add about Amazon CloudWatch alarms when the deployment
          group is            created
        type: string
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Configuration information for an automatic rollback that is added
          when a deployment            group is created
        type: string
      - in: query
        name: autoScalingGroups
        description: A list of associated Auto Scaling groups
        type: string
      - in: query
        name: deploymentConfigName
        description: If specified, the deployment configuration name can be either
          one of the predefined            configurations provided with AWS CodeDeploy
          or a custom deployment configuration that            you create by calling
          the create deployment configuration operation
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of a new deployment group for the specified application
        type: string
      - in: query
        name: ec2TagFilters
        description: The Amazon EC2 tags on which to filter
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The on-premises instance tags on which to filter
        type: string
      - in: query
        name: serviceRoleArn
        description: A service role ARN that allows AWS CodeDeploy to act on the users
          behalf when            interacting with AWS services
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to create when the deployment group
          is created
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=DeleteDeploymentGroup:
    get:
      summary: Delete Deployment Group
      description: Deletes a deployment group.
      operationId: deleteDeploymentGroup
      x-api-path-slug: actiondeletedeploymentgroup-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=GetDeploymentGroup:
    get:
      summary: Get Deployment Group
      description: Gets information about a deployment group.
      operationId: getDeploymentGroup
      x-api-path-slug: actiongetdeploymentgroup-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: deploymentGroupName
        description: The name of an existing deployment group for the specified application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
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