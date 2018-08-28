---
name: IBM Cloud
x-slug: ibm-cloud
description: The IBM Cloud has been built to help you solve problems and advance opportunities
  in a world flush with data. Whether it&rsquo;s data you possess, data outside your
  firewall, or data that&rsquo;s coming, the IBM Cloud helps you protect it, move
  it, integrate it and unlock intelligence from it &mdash; giving you what it takes
  to prevail in a competitive market.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
x-kinRank: "8"
x-alexaRank: "11207"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/apis.md
specificationVersion: "0.14"
apis:
- name: IBM Containers - List all container groups in a space
  x-api-slug: containersgroups-get
  description: 'This endpoint returns a list of all container groups in a space independent
    of their current state. (corresponding IBM Containers command: `cf ic group list`).'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroups-get-openapi.md
- name: IBM Containers - Create and start a container group.
  x-api-slug: containersgroups-post
  description: "This endpoint creates and starts a new container group in your space.
    A container group consists of two or more single containers that are all created
    from the same container image and as a consequence are configured in the same
    way. Container groups offer different options at no cost to make your app highly
    available, such as in-built load balancing, auto-recovery of unhealthy container
    instances, and auto-scaling of container instances based on CPU and memory usage.\n\nTo
    create a container group with IBM Containers, you must at least define a container
    group name and the image that the container group is based on. Required attributes:\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n-
    Name: The container group name must start with a letter and then can include uppercase
    letters, lowercase letters, numbers, periods (.), underscores (_), or hyphens
    (-). \n- Image: You must include the full path to the image in your private Bluemix
    registry in the format:`registry.ng.bluemix.net/<namespace>/<image>`."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroups-post-openapi.md
- name: IBM Containers - Stop and delete all container instances in a container group.
  x-api-slug: containersgroupsname-or-id-delete
  description: 'Stops and deletes the container instances that run in a container
    group (corresponding IBM Containers command: `cf ic group rm <group_name>`). When
    you delete a container group, all floating private IP addresses are released.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroupsname-or-id-delete-openapi.md
- name: IBM Containers - Inspect a container group.
  x-api-slug: containersgroupsname-or-id-get
  description: 'This endpoint retrieves detailed information about a container group
    with a given name (corresponding IBM Containers command: `cf ic group inspect
    GROUP`).'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroupsname-or-id-get-openapi.md
- name: IBM Containers - Update a container group.
  x-api-slug: containersgroupsname-or-id-patch
  description: "Update the number of container instances that run in a container group
    (corresponding IBM Containers command: `cf ic group update <option> <group>`).
    \n\nNote: You can run only one update at a time.  \n\n The desired number is the
    number of container instances that you require. It must be within the current
    limits of Max and Min. To increase the number of desired container instances above
    the Max value, you must first execute an update on the Max value. Once this update
    is completed, you can increase the desired number of container instances."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroupsname-or-id-patch-openapi.md
- name: IBM Containers - Map a public route to a container group.
  x-api-slug: containersgroupsname-or-idmaproute-post
  description: 'If you want your container group to be accessible from the Internet,
    you need to expose a public port and map a public route to it (corresponding IBM
    Containers command: `cf ic route map -n <host> -d <domain> <group>`). Every route
    consists of the host name and domain.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroupsname-or-idmaproute-post-openapi.md
- name: IBM Containers - Unmap a public route from a container group
  x-api-slug: containersgroupsname-or-idunmaproute-post
  description: "This endpoint unmaps a public route from a container group (corresponding
    IBM Containers command: `cf ic route unmap -n <host> -d <domain> <group>`). If
    no other public route is mapped to the container group, then the container group
    is no longer available from the internet. \n\n When you unmap a route from a container
    group, the route is not deleted and can be mapped to other container groups."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28560-ibm-containers.jpg
  humanURL: https://www.ibm.com/cloud/
  baseURL: https://containers-api.ng.bluemix.net//v3
  tags: SaaS, Technology, Enterprise, API Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/ibm-cloud/containersgroupsname-or-idunmaproute-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://hsbc.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ibm.cloud.stack.network
- type: x-blog
  url: https://www.ibm.com/blogs/bluemix/
- type: x-crunchbase
  url: https://crunchbase.com/organization/product/ibm-bluemix
- type: x-github
  url: https://github.com/IBM-Cloud
- type: x-twitter
  url: https://twitter.com/IBMcloud
- type: x-website
  url: https://www.ibm.com/cloud/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---