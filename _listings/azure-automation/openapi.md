swagger: "2.0"
x-collection-name: Azure Automation
x-complete: 1
info:
  title: AutomationManagementClient
  version: 1.0.0
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