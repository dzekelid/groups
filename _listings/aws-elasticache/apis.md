---
name: AWS ElastiCache
x-slug: aws-elasticache
description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
  and scale an in-memory data store or cache in the cloud. The service improves the
  performance of web applications by allowing you to retrieve information from fast,
  managed, in-memory data stores, instead of relying entirely on slower disk-based
  databases. Amazon ElastiCache automatically detects and replaces failed nodes, reducing
  the overhead associated with self-managed infrastructures and provides a resilient
  system that mitigates the risk of overloaded databases, which slow website and application
  load times. Through integration with Amazon CloudWatch, Amazon ElastiCache provides
  enhanced visibility into key performance metrics associated with your Redis or Memcached
  nodes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon ElastiCache API Authorize Cache Security Group Ingress
  x-api-slug: amazon-elasticache-api
  description: |-
    Allows network ingress to a cache
                security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=AuthorizeCacheSecurityGroupIngress
  tags: Cache Security Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionauthorizecachesecuritygroupingress-get-openapi.md
- name: Amazon ElastiCache API Create Cache Parameter Group
  x-api-slug: amazon-elasticache-api
  description: Creates a new cache parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CreateCacheParameterGroup
  tags: Cache Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actioncreatecacheparametergroup-get-openapi.md
- name: Amazon ElastiCache API Create Cache Security Group
  x-api-slug: amazon-elasticache-api
  description: Creates a new cache security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CreateCacheSecurityGroup
  tags: Cache Security Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actioncreatecachesecuritygroup-get-openapi.md
- name: Amazon ElastiCache API Create Cache Subnet Group
  x-api-slug: amazon-elasticache-api
  description: Creates a new cache subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CreateCacheSubnetGroup
  tags: Cache Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actioncreatecachesubnetgroup-get-openapi.md
- name: Amazon ElastiCache API Create Replication Group
  x-api-slug: amazon-elasticache-api
  description: Creates a Redis (cluster mode disabled) or a Redis (cluster mode enabled)
    replication group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=CreateReplicationGroup
  tags: Replication Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actioncreatereplicationgroup-get-openapi.md
- name: Amazon ElastiCache API Delete Cache Parameter Group
  x-api-slug: amazon-elasticache-api
  description: |-
    Deletes the specified cache parameter
                group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DeleteCacheParameterGroup
  tags: Cache Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondeletecacheparametergroup-get-openapi.md
- name: Amazon ElastiCache API Delete Cache Security Group
  x-api-slug: amazon-elasticache-api
  description: Deletes a cache security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DeleteCacheSecurityGroup
  tags: Cache Security Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondeletecachesecuritygroup-get-openapi.md
- name: Amazon ElastiCache API Delete Cache Subnet Group
  x-api-slug: amazon-elasticache-api
  description: Deletes a cache subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DeleteCacheSubnetGroup
  tags: Cache Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondeletecachesubnetgroup-get-openapi.md
- name: Amazon ElastiCache API Delete Replication Group
  x-api-slug: amazon-elasticache-api
  description: Deletes an existing replication group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DeleteReplicationGroup
  tags: Replication Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondeletereplicationgroup-get-openapi.md
- name: Amazon ElastiCache API Describe Cache Parameter Groups
  x-api-slug: amazon-elasticache-api
  description: |-
    Returns a list of cache parameter group
                descriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeCacheParameterGroups
  tags: Cache Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondescribecacheparametergroups-get-openapi.md
- name: Amazon ElastiCache API Describe Cache Security Groups
  x-api-slug: amazon-elasticache-api
  description: |-
    Returns a list of cache security group
                descriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeCacheSecurityGroups
  tags: Cache Security Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondescribecachesecuritygroups-get-openapi.md
- name: Amazon ElastiCache API Describe Cache Subnet Groups
  x-api-slug: amazon-elasticache-api
  description: |-
    Returns a list of cache subnet group
                descriptions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeCacheSubnetGroups
  tags: Cache Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondescribecachesubnetgroups-get-openapi.md
- name: Amazon ElastiCache API Describe Replication Groups
  x-api-slug: amazon-elasticache-api
  description: |-
    Returns information about a particular
                replication group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=DescribeReplicationGroups
  tags: Replication Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actiondescribereplicationgroups-get-openapi.md
- name: Amazon ElastiCache API Modify Cache Parameter Group
  x-api-slug: amazon-elasticache-api
  description: |-
    Modifies the parameters of a cache
                parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=ModifyCacheParameterGroup
  tags: Cache Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionmodifycacheparametergroup-get-openapi.md
- name: Amazon ElastiCache API Modify Cache Subnet Group
  x-api-slug: amazon-elasticache-api
  description: Modifies an existing cache subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=ModifyCacheSubnetGroup
  tags: Cache Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionmodifycachesubnetgroup-get-openapi.md
- name: Amazon ElastiCache API Modify Replication Group
  x-api-slug: amazon-elasticache-api
  description: Modifies the settings for a replication group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=ModifyReplicationGroup
  tags: Replication Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionmodifyreplicationgroup-get-openapi.md
- name: Amazon ElastiCache API Reset Cache Parameter Group
  x-api-slug: amazon-elasticache-api
  description: |-
    Modifies the parameters of a cache
                parameter group to the engine or system default value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=ResetCacheParameterGroup
  tags: Cache Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionresetcacheparametergroup-get-openapi.md
- name: Amazon ElastiCache API Revoke Cache Security Group Ingress
  x-api-slug: amazon-elasticache-api
  description: |-
    Revokes ingress from a cache
                security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: ://///?Action=RevokeCacheSecurityGroupIngress
  tags: Cache Security Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/actionrevokecachesecuritygroupingress-get-openapi.md
- name: Amazon ElastiCache API
  x-api-slug: amazon-elasticache-api
  description: Amazon ElastiCache is a web service that makes it easy to deploy, operate,
    and scale an in-memory data store or cache in the cloud. The service improves
    the performance of web applications by allowing you to retrieve information from
    fast, managed, in-memory data stores, instead of relying entirely on slower disk-based
    databases. Amazon ElastiCache automatically detects and replaces failed nodes,
    reducing the overhead associated with self-managed infrastructures and provides
    a resilient system that mitigates the risk of overloaded databases, which slow
    website and application load times. Through integration with Amazon CloudWatch,
    Amazon ElastiCache provides enhanced visibility into key performance metrics associated
    with your Redis or Memcached nodes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonElasticCache.png
  humanURL: https://aws.amazon.com/elasticache/
  baseURL: :///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/aws-elasticache/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonElastiCache/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/elasticache/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/elasticache/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/elasticache/pricing/
- type: x-resources
  url: https://aws.amazon.com/elasticache/developer-resources/
- type: x-testimonials
  url: https://aws.amazon.com/elasticache/testimonials/
- type: x-website
  url: https://aws.amazon.com/elasticache/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---