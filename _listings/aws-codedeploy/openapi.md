---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 1
info:
  title: AWS CodeDeploy API
  version: 1.0.0
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
  /?Action=ListDeploymentGroups:
    get:
      summary: List Deployment Groups
      description: |-
        Lists the deployment groups for an application registered with the applicable IAM
                    user or AWS account.
      operationId: listDeploymentGroups
      x-api-path-slug: actionlistdeploymentgroups-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment groups
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
  /?Action=UpdateDeploymentGroup:
    get:
      summary: Update Deployment Group
      description: Changes information about a deployment group.
      operationId: updateDeploymentGroup
      x-api-path-slug: actionupdatedeploymentgroup-get
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add or change about Amazon CloudWatch alarms when
          the deployment            group is updated
        type: string
      - in: query
        name: applicationName
        description: The application name corresponding to the deployment group to
          update
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Information for an automatic rollback configuration that is added
          or changed when a            deployment group is updated
        type: string
      - in: query
        name: autoScalingGroups
        description: The replacement list of Auto Scaling groups to be included in
          the deployment group,            if you want to change them
        type: string
      - in: query
        name: currentDeploymentGroupName
        description: The current name of the deployment group
        type: string
      - in: query
        name: deploymentConfigName
        description: The replacement deployment configuration name to use, if you
          want to change            it
        type: string
      - in: query
        name: ec2TagFilters
        description: The replacement set of Amazon EC2 tags on which to filter, if
          you want to change            them
        type: string
      - in: query
        name: newDeploymentGroupName
        description: The new name of the deployment group, if you want to change it
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The replacement set of on-premises instance tags on which to
          filter, if you want to            change them
        type: string
      - in: query
        name: serviceRoleArn
        description: A replacement ARN for the service role, if you want to change
          it
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to change when the deployment group
          is updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
---