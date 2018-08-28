---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 1
info:
  title: CloudFlare
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups:
    get:
      summary: Search, list, and sort rule groups contained within a package
      description: Search, list, and sort rule groups contained within a package
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroups-get
      parameters:
      - in: query
        name: direction
        description: Direction to order groupsttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: Whether or not the rules contained within this group are configurable/usabletttttttttttttton
      - in: query
        name: name
        description: Name of the firewall rule groupttttttttttttttProject Honey Pot
      - in: query
        name: order
        description: Field to order groups byttttttttttttttmode
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of groups per pagetttttttttttttt50
      - in: query
        name: rules_count
        description: How many rules are contained within this grouptttttttttttttt10
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
  /zones/:zone_identifier/firewall/waf/packages/:package_identifier/groups/:identifier:
    get:
      summary: Get a single rule group
      description: Get a single rule group
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
    patch:
      summary: Update the state of a rule group
      description: Update the state of a rule group
      operationId: cloudflare-waf-rule-groups-api
      x-api-path-slug: zoneszone-identifierfirewallwafpackagespackage-identifiergroupsidentifier-patch
      parameters:
      - in: query
        name: mode
        description: Whether or not the rules contained within this group are configurable/usabletttttttttttttton
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - WAF Rule Groups
---