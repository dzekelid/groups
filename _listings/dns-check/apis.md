---
name: DNS Check
x-slug: dns-check
description: Monitor DNS records. Request DNS updates by sharing reports that show
  the pass/fail status of each record. Troubleshoot DNS issues. DNS records are automatically
  re-checked, and reports updated. DNS records can be imported from a zone file, or
  added in...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18972-dns-check.jpg
x-kinRank: "8"
x-alexaRank: "3315601"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/dns-check/apis.md
specificationVersion: "0.14"
apis:
- name: DNS Record Group Monitoring API - Check Group
  x-api-slug: groupsgroup-uuid-get
  description: The DNS Check API is used to request data for either a specific record
    group, or all DNS record groups owned by your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18972-dns-check.jpg
  humanURL: https://www.dnscheck.co/
  baseURL: https://www.dnscheck.co//api/v1
  tags: dns check, dns monitor, DNS, mx record check, spf record check, DNS General,
    Monitoring, Stack Network, Technology, SaaS, API Provider, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/dns-check/groupsgroup-uuid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://disqus.api.gallery.streamdata.io
- type: x-api-stack
  url: http://dns.check.stack.network
- type: x-developer
  url: https://www.dnscheck.co/documentation
- type: x-pricing
  url: https://www.dnscheck.co/pricing
- type: x-twitter
  url: https://twitter.com/dns_check
- type: x-website
  url: https://www.dnscheck.co/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---