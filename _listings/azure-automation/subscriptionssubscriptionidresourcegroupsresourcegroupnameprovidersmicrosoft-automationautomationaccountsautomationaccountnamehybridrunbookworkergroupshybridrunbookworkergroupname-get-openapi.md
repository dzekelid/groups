---
swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 0
info:
  title: Azure Automation API Hybrid Runbook Worker Group Get
  version: 1.0.0
  description: Retrieve a hybrid runbook worker group.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts:
    get:
      summary: Automation Account List By Resource Group
      description: Retrieve a list of accounts within a given resource group.
      operationId: AutomationAccount_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Automation
      - Account
      - List
      - Resource
      - Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/hybridRunbookWorkerGroups/{hybridRunbookWorkerGroupName}
  : delete:
      summary: Hybrid Runbook Worker Group Delete
      description: Delete a hybrid runbook worker group.
      operationId: HybridRunbookWorkerGroup_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamehybridrunbookworkergroupshybridrunbookworkergroupname-delete
      parameters:
      - in: path
        name: automationAccountName
        description: Automation account name
      - in: path
        name: hybridRunbookWorkerGroupName
        description: The hybrid runbook worker group name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hybrid
      - Runbook
      - Worker
      - Group
    get:
      summary: Hybrid Runbook Worker Group Get
      description: Retrieve a hybrid runbook worker group.
      operationId: HybridRunbookWorkerGroup_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamehybridrunbookworkergroupshybridrunbookworkergroupname-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: hybridRunbookWorkerGroupName
        description: The hybrid runbook worker group name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hybrid
      - Runbook
      - Worker
      - Group
    patch:
      summary: Hybrid Runbook Worker Group Update
      description: Update a hybrid runbook worker group.
      operationId: HybridRunbookWorkerGroup_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamehybridrunbookworkergroupshybridrunbookworkergroupname-patch
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: path
        name: hybridRunbookWorkerGroupName
        description: The hybrid runbook worker group name
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The hybrid runbook worker group
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hybrid
      - Runbook
      - Worker
      - Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Automation/automationAccounts/{automationAccountName}/hybridRunbookWorkerGroups
  : get:
      summary: Hybrid Runbook Worker Group List By Automation Account
      description: Retrieve a list of hybrid runbook worker groups.
      operationId: HybridRunbookWorkerGroup_ListByAutomationAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-automationautomationaccountsautomationaccountnamehybridrunbookworkergroups-get
      parameters:
      - in: path
        name: automationAccountName
        description: The automation account name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Hybrid
      - Runbook
      - Worker
      - Group
      - List
      - Automation
      - Account
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