---
name: AWS Cognito
x-slug: aws-cognito
description: Amazon Cognito lets you easily add user sign-up and sign-in to your mobile
  and web apps. With Amazon Cognito, you also have the options to authenticate users
  through social identity providers such as Facebook, Twitter, or Amazon, with SAML
  identity solutions, or by using your own identity system. In addition, Amazon Cognito
  enables you to save data locally on users devices, allowing your applications to
  work even when the devices are offline. You can then synchronize data across users
  devices so that their app experience remains consistent regardless of the device
  they use. With Amazon Cognito, you can focus on creating great app experiences instead
  of worrying about building, securing, and scaling a solution to handle user management,
  authentication, and sync across devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Cognito API Admin Add User To Group
  x-api-slug: aws-cognito-api
  description: Adds the specified user to the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminAddUserToGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminaddusertogroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminaddusertogroup-get-openapi.md
- name: AWS Cognito API Admin List Groups For User
  x-api-slug: aws-cognito-api
  description: Lists the groups that the user belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminListGroupsForUser
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminlistgroupsforuser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminlistgroupsforuser-get-openapi.md
- name: AWS Cognito API Admin Remove User From Group
  x-api-slug: aws-cognito-api
  description: Removes the specified user from the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=AdminRemoveUserFromGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminremoveuserfromgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionadminremoveuserfromgroup-get-openapi.md
- name: AWS Cognito API Create Group
  x-api-slug: aws-cognito-api
  description: Creates a new group in the specified user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=CreateGroup
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actioncreategroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actioncreategroup-get-openapi.md
- name: AWS Cognito API Delete Group
  x-api-slug: aws-cognito-api
  description: Deletes a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=DeleteGroup
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actiondeletegroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actiondeletegroup-get-openapi.md
- name: AWS Cognito API Get Group
  x-api-slug: aws-cognito-api
  description: Gets a group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=GetGroup
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actiongetgroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actiongetgroup-get-openapi.md
- name: AWS Cognito API List Groups
  x-api-slug: aws-cognito-api
  description: Lists the groups associated with a user pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListGroups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionlistgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionlistgroups-get-openapi.md
- name: AWS Cognito API List Users In Group
  x-api-slug: aws-cognito-api
  description: Lists the users in the specified group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=ListUsersInGroup
  tags: Users,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionlistusersingroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionlistusersingroup-get-openapi.md
- name: AWS Cognito API Update Group
  x-api-slug: aws-cognito-api
  description: Updates the specified group with the specified attributes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https://///?Action=UpdateGroup
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionupdategroup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/actionupdategroup-get-openapi.md
- name: AWS Cognito API
  x-api-slug: aws-cognito-api
  description: Amazon Cognito lets you easily add user sign-up and sign-in to your
    mobile and web apps. With Amazon Cognito, you also have the options to authenticate
    users through social identity providers such as Facebook, Twitter, or Amazon,
    with SAML identity solutions, or by using your own identity system. In addition,
    Amazon Cognito enables you to save data locally on users devices, allowing your
    applications to work even when the devices are offline. You can then synchronize
    data across users devices so that their app experience remains consistent regardless
    of the device they use. With Amazon Cognito, you can focus on creating great app
    experiences instead of worrying about building, securing, and scaling a solution
    to handle user management, authentication, and sync across devices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-cognito.png
  humanURL: https://aws.amazon.com/cognito/
  baseURL: https:///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-cognito/openapi.md
x-common:
- type: x-blog
  url: https://aws.amazon.com/cognito/dev-resources/#blogposts
- type: x-documentation
  url: http://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitoidentity/latest/APIReference/Welcome.html
- type: x-documentation
  url: http://docs.aws.amazon.com/cognitosync/latest/APIReference/Welcome.html
- type: x-faq
  url: http://aws.amazon.com/cognito/faqs
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=173
- type: x-pricing
  url: http://aws.amazon.com/cognito/pricing
- type: x-sdk
  url: https://aws.amazon.com/cognito/dev-resources/#documentation
- type: x-slides
  url: https://aws.amazon.com/cognito/dev-resources/#slides
- type: x-videos
  url: https://aws.amazon.com/cognito/dev-resources/#videos
- type: x-website
  url: https://aws.amazon.com/cognito/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---