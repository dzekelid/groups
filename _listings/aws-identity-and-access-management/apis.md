---
name: AWS Identity and Access Management
x-slug: aws-identity-and-access-management
description: AWS Identity and Access Management (IAM) enables you to securely control
  access to AWS services and resources for your users. Using IAM, you can create and
  manage AWS users and groups, and use permissions to allow and deny their access
  to AWS resources.IAM is a feature of your AWS account offered at no additional charge.
  You will be charged only for use of other AWS services by your users.To get started
  using IAM, orif you have already registered with AWS, go to theAWS Management Consoleand
  get started with theseIAM Best Practices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Identity and Access Management API Add User To Group
  x-api-slug: aws-identity-and-access-management-api
  description: Adds the specified user to the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=AddUserToGroup
  tags: User Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actionaddusertogroup-get-openapi.md
- name: AWS Identity and Access Management API Create Group
  x-api-slug: aws-identity-and-access-management-api
  description: Creates a new group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=CreateGroup
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actioncreategroup-get-openapi.md
- name: AWS Identity and Access Management API Delete Group
  x-api-slug: aws-identity-and-access-management-api
  description: Deletes the specified IAM group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=DeleteGroup
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actiondeletegroup-get-openapi.md
- name: AWS Identity and Access Management API Get Group
  x-api-slug: aws-identity-and-access-management-api
  description: Returns a list of IAM users that are in the specified IAM group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=GetGroup
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actiongetgroup-get-openapi.md
- name: AWS Identity and Access Management API List Groups
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the IAM groups that have the specified path prefix.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListGroups
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actionlistgroups-get-openapi.md
- name: AWS Identity and Access Management API List Groups For User
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the IAM groups that the specified IAM user belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListGroupsForUser
  tags: Groups For User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actionlistgroupsforuser-get-openapi.md
- name: AWS Identity and Access Management API Remove User From Group
  x-api-slug: aws-identity-and-access-management-api
  description: Removes the specified user from the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=RemoveUserFromGroup
  tags: User From Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actionremoveuserfromgroup-get-openapi.md
- name: AWS Identity and Access Management API Update Group
  x-api-slug: aws-identity-and-access-management-api
  description: Updates the name and/or the path of the specified IAM group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UpdateGroup
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/actionupdategroup-get-openapi.md
- name: AWS Identity and Access Management API
  x-api-slug: aws-identity-and-access-management-api
  description: AWS Identity and Access Management (IAM) enables you to securely control
    access to AWS services and resources for your users. Using IAM, you can create
    and manage AWS users and groups, and use permissions to allow and deny their access
    to AWS resources.IAM is a feature of your AWS account offered at no additional
    charge. You will be charged only for use of other AWS services by your users.To
    get started using IAM, orif you have already registered with AWS, go to theAWS
    Management Consoleand get started with theseIAM Best Practices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-identity-and-access-management/openapi.md
x-common:
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=323
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sts/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/IAM/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/iam/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=76
- type: x-getting-started
  url: https://aws.amazon.com/iam/getting-started/
- type: x-partners
  url: https://aws.amazon.com/iam/partners/
- type: x-tools
  url: http://aws.amazon.com/cli
- type: x-website
  url: https://aws.amazon.com/iam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---