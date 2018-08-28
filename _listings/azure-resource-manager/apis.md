---
name: Azure Resource Manager
x-slug: azure-resource-manager
description: Azure Resource Manager enables you to deploy and manage the infrastructure
  for your Azure solutions. You organize related resources in resource groups, and
  deploy your resources with JSON templates. For an introduction to deploying and
  managing resources with Resource Manager, see Azure Resource Manager overview.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Resource Manager API Resource Groups List Resources
  x-api-slug: azure-resource-manager-api
  description: Get all the resources for a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/resources
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameresources-get-openapi.md
- name: Azure Resource Manager API Resource Groups Check Existence
  x-api-slug: azure-resource-manager-api
  description: Checks whether a resource group exists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups Existence
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-head-openapi.md
- name: Azure Resource Manager API Resource Groups Create Or Update
  x-api-slug: azure-resource-manager-api
  description: Creates a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-put-openapi.md
- name: Azure Resource Manager API Resource Groups Get
  x-api-slug: azure-resource-manager-api
  description: Gets a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupname-get-openapi.md
- name: Azure Resource Manager API Resource Groups Export Template
  x-api-slug: azure-resource-manager-api
  description: Captures the specified resource group as a template.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/exportTemplate
  tags: Resource Groups Export Template
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroupsresourcegroupnameexporttemplate-post-openapi.md
- name: Azure Resource Manager API Resource Groups List
  x-api-slug: azure-resource-manager-api
  description: Gets all the resource groups for a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourcegroups
  tags: Resource Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/subscriptionssubscriptionidresourcegroups-get-openapi.md
- name: Azure Resource Manager API
  x-api-slug: azure-resource-manager-api
  description: Azure Resource Manager enables you to deploy and manage the infrastructure
    for your Azure solutions. You organize related resources in resource groups, and
    deploy your resources with JSON templates. For an introduction to deploying and
    managing resources with Resource Manager, see Azure Resource Manager overview.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-resource-manager.png
  humanURL: https://docs.microsoft.com/en-us/rest/api/resources/
  baseURL: ://management.azure.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/azure-resource-manager/openapi.md
x-common:
- type: x-website
  url: https://docs.microsoft.com/en-us/rest/api/resources/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---