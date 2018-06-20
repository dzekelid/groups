---
name: CloudFlare
x-slug: cloudflare
description: Here at Cloudflare, we make the Internet work the way it should. Offering
  CDN, DNS, DDoS protection and security, find out how we can help your site.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18929-cloudflare.jpg
x-kinRank: "9"
x-alexaRank: "1685"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/apis.md
specificationVersion: "0.14"
apis:
- name: CloudFlare Search, list, and sort rule groups contained within a package
  x-api-slug: cloudflare
  description: Search, list, and sort rule groups contained within a package
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18929-cloudflare.jpg
  humanURL: https://www.cloudflare.com
  baseURL: https://///zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups
  tags: WAF Rule Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroups-get-openapi.md
- name: CloudFlare Get a single rule group
  x-api-slug: cloudflare
  description: Get a single rule group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18929-cloudflare.jpg
  humanURL: https://www.cloudflare.com
  baseURL: https://///zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier
  tags: WAF Rule Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-get-openapi.md
- name: CloudFlare Update the state of a rule group
  x-api-slug: cloudflare
  description: Update the state of a rule group
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18929-cloudflare.jpg
  humanURL: https://www.cloudflare.com
  baseURL: https://///zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier
  tags: WAF Rule Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-patch-openapi.md
- name: CloudFlare
  x-api-slug: cloudflare
  description: Here at Cloudflare, we make the Internet work the way it should. Offering
    CDN, DNS, DDoS protection and security, find out how we can help your site.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18929-cloudflare.jpg
  humanURL: https://www.cloudflare.com
  baseURL: https:///
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/cloudflare/openapi.md
x-common:
- type: x-blog
  url: https://blog.cloudflare.com/
- type: x-blog-rss
  url: http://blog.cloudflare.com/rss/
- type: x-crunchbase
  url: https://crunchbase.com/organization/cloudflare
- type: x-developer
  url: https://www.cloudflare.com/docs/client-api.html
- type: x-github
  url: https://github.com/cloudflare
- type: x-partners
  url: https://www.cloudflare.com/partners/
- type: x-pricing
  url: https://www.cloudflare.com/plans/
- type: x-privacy
  url: https://www.cloudflare.com/security-policy
- type: x-security
  url: https://www.cloudflare.com/security-policy/
- type: x-terms-of-service
  url: https://www.cloudflare.com/terms/
- type: x-transparency-report
  url: https://www.cloudflare.com/transparency/
- type: x-twitter
  url: https://twitter.com/CloudFlare
- type: x-website
  url: https://www.cloudflare.com
- type: x-website
  url: http://cloudflare.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---