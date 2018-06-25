---
name: AWS Redshift
x-slug: aws-redshift
description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
  makes it simple and cost-effective to analyze all your data using your existing
  business intelligence tools. Start small for $0.25 per hour with no commitments
  and scale to petabytes for $1,000 per terabyte per year, less than a tenth the cost
  of traditional solutions. Customers typically see 3x compression, reducing their
  costs to $333 per uncompressed terabyte per year.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Redshift API Create Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Creates an Amazon Redshift parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actioncreateclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Create Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Creates a new Amazon Redshift subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actioncreateclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Delete Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Deletes a specified Amazon Redshift parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actiondeleteclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Delete Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Deletes the specified cluster subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actiondeleteclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Describe Cluster Parameter Groups
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of Amazon Redshift parameter groups, including parameter groups you
                created and the default parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterParameterGroups
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actiondescribeclusterparametergroups-get-openapi.md
- name: Amazon Redshift API Describe Cluster Subnet Groups
  x-api-slug: amazon-redshift-api
  description: |-
    Returns one or more cluster subnet group objects, which contain metadata about your
                cluster subnet groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSubnetGroups
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actiondescribeclustersubnetgroups-get-openapi.md
- name: Amazon Redshift API Modify Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Modifies the parameters of a parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actionmodifyclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Modify Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Modifies a cluster subnet group to include the specified list of VPC
    subnets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actionmodifyclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Reset Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: |-
    Sets one or more parameters of the specified parameter group to their default
                values and sets the source values of the parameters to "engine-default".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ResetClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/actionresetclusterparametergroup-get-openapi.md
- name: Amazon Redshift API
  x-api-slug: amazon-redshift-api
  description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
    makes it simple and cost-effective to analyze all your data using your existing
    business intelligence tools. Start small for $0.25 per hour with no commitments
    and scale to petabytes for $1,000 per terabyte per year, less than a tenth the
    cost of traditional solutions. Customers typically see 3x compression, reducing
    their costs to $333 per uncompressed terabyte per year.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: :///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-redshift/openapi.md
x-common:
- type: x-best-practices
  url: https://aws.amazon.com/redshift/developer-resources/#best-practices
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/redshift/index.html
- type: x-customer-success
  url: https://aws.amazon.com/redshift/customer-success/
- type: x-documentation
  url: http://docs.aws.amazon.com/redshift/latest/APIReference/
- type: x-events
  url: https://aws.amazon.com/redshift/events/
- type: x-faq
  url: https://aws.amazon.com/redshift/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/redshift/getting-started/
- type: x-partners
  url: https://aws.amazon.com/redshift/partners/
- type: x-pricing
  url: https://aws.amazon.com/redshift/pricing/
- type: x-website
  url: https://aws.amazon.com/redshift/
- type: x-whats-new
  url: https://aws.amazon.com/redshift/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---