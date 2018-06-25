---
name: AWS Inspector
x-slug: aws-inspector
description: Amazon Inspector is an automated security assessment service that helps
  improve the security and compliance of applications deployed on AWS. Amazon Inspector
  automatically assesses applications for vulnerabilities or deviations from best
  practices. After performing an assessment, Amazon Inspector produces a detailed
  list of security findings prioritized by level of severity.To help you get started
  quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped
  to common security best practices and vulnerability definitions. Examples of built-in
  rules include checking for remote root login being enabled, or vulnerable software
  versions installed. These rules are regularly updated by AWS security researchers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-inspector/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Inspector API Create Resource Group
  x-api-slug: aws-inspector-api
  description: |-
    Creates a resource group using the specified set of tags (key and value pairs) that
             are used to select the EC2 instances to be included in an Amazon Inspector assessment
             target.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: ://///?Action=CreateResourceGroup
  tags: Resource Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-inspector/actioncreateresourcegroup-get-openapi.md
- name: AWS Inspector API Describe Resource Groups
  x-api-slug: aws-inspector-api
  description: |-
    Describes the resource groups that are specified by the ARNs of the resource
             groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: ://///?Action=DescribeResourceGroups
  tags: Resource Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-inspector/actiondescriberesourcegroups-get-openapi.md
- name: AWS Inspector API
  x-api-slug: aws-inspector-api
  description: Amazon Inspector is an automated security assessment service that helps
    improve the security and compliance of applications deployed on AWS. Amazon Inspector
    automatically assesses applications for vulnerabilities or deviations from best
    practices. After performing an assessment, Amazon Inspector produces a detailed
    list of security findings prioritized by level of severity.To help you get started
    quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped
    to common security best practices and vulnerability definitions. Examples of built-in
    rules include checking for remote root login being enabled, or vulnerable software
    versions installed. These rules are regularly updated by AWS security researchers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AmazonInspector.png
  humanURL: https://aws.amazon.com/inspector/
  baseURL: :///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-inspector/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/inspector/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/inspector/faqs/
- type: x-getting-started
  url: https://docs.aws.amazon.com/inspector/latest/userguide/inspector_quickstart.html
- type: x-partners
  url: https://aws.amazon.com/inspector/partners/
- type: x-pricing
  url: https://aws.amazon.com/inspector/pricing/
- type: x-testimonials
  url: https://aws.amazon.com/inspector/customers/
- type: x-website
  url: https://aws.amazon.com/inspector/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---