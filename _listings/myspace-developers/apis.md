---
name: MySpace Developers
x-slug: myspace-developers
description: 'AskMyspace: http://askmyspace.com  Twitter: http://twitter.com/Myspace  Instagram:
  http://instagram.com/Myspace  Tumblr: http://myspace.tumblr.com  YouTube: http://www.youtube.com/Myspace'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1619-myspace-developers.jpg
x-kinRank: "7"
x-alexaRank: "4691"
tags: Groups
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/apis.md
specificationVersion: "0.14"
apis:
- name: My Space Get Groups Personid
  x-api-slug: my-space
  description: Retrieves the current user's groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1619-myspace-developers.jpg
  humanURL: http://wiki.developer.myspace.com/index.php?title=Category:RESTful_API
  baseURL: https://api.myspace.com////1.0/groups/{personId}
  tags: Groups,People
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/1-0groupspersonid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/1-0groupspersonid-get-openapi.md
- name: My Space Get Groups Supported Fields
  x-api-slug: my-space
  description: Retrieves all supported fields.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1619-myspace-developers.jpg
  humanURL: http://wiki.developer.myspace.com/index.php?title=Category:RESTful_API
  baseURL: https://api.myspace.com////1.0/groups/@supportedFields
  tags: Groups,Supported,Fields
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/1-0groupssupportedfields-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/1-0groupssupportedfields-get-openapi.md
- name: My Space
  x-api-slug: my-space
  description: 'AskMyspace: http://askmyspace.com  Twitter: http://twitter.com/Myspace  Instagram:
    http://instagram.com/Myspace  Tumblr: http://myspace.tumblr.com  YouTube: http://www.youtube.com/Myspace'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1619-myspace-developers.jpg
  humanURL: http://wiki.developer.myspace.com/index.php?title=Category:RESTful_API
  baseURL: https://api.myspace.com//
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/myspace-developers/openapi.md
x-common:
- type: x-website
  url: http://wiki.developer.myspace.com/index.php?title=Category:RESTful_API
- type: x-blog
  url: http://www.myspace.com/pressroom?url=/company+blog/
- type: x-blog-rss
  url: http://myspace.tekgroupweb.com/company+blog/rss.xml
- type: x-crunchbase
  url: http://www.crunchbase.com/company/myspace
- type: x-crunchbase
  url: https://crunchbase.com/organization/myspace
- type: x-github
  url: https://github.com/myspace
- type: x-twitter
  url: https://twitter.com/#!/MySpaceDevTeam
- type: x-twitter
  url: https://twitter.com/Myspace
- type: x-website
  url: http://myspace.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---