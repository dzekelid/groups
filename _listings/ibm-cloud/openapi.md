---
swagger: "2.0"
x-collection-name: IBM Cloud
x-complete: 1
info:
  title: IBM Containers
  description: containers-are-virtual-software-objects-that-include-all-the-elements-that-an-app-needs-to-run--a-container-has-the-benefits-of-resource-isolation-and-allocation-but-is-more-portable-and-efficient-than-for-example-a-virtual-machine--this-documentation-describes-the-ibm-containers-api-which-is-based-on-the-docker-remote-api--the-api-provides-endpoints-that-you-can-use-to-create-and-manage-your-single-containers-and-container-groups-in-bluemix--endpoints-are-summarized-under-the-following-tags--authentication-retrieve-and-refresh-your-tls-certificates---private-docker-images-registry-create-your-own-private-docker-images-registry-in-bluemix-by-setting-a-namespace-for-your-organization---images-view-build-and-push-your-images-to-your-private-bluemix-registry-so-you-can-use-them-with-ibm-containers--you-can-also-scan-your-container-images-with-the-vulnerability-advisor-against-standard-policies-set-by-the-organization-manager-and-a-database-of-known-ubuntu-issues---single-containers-create-and-manage-single-containers-in-bluemix--use-a-single-container-to-implement-shortlived-processes-or-to-run-simple-tests-as-you-develop-an-app-or-service--to-make-your-single-container-available-from-the-internet-review-the-public-ip-addresses-endpoints---container-groups-create-and-manage-your-container-groups-in-bluemix--a-container-group-consists-of-multiple-single-containers-that-are-all-created-from-the-same-container-image-and-as-a-consequence-are-configured-in-the-same-way--container-groups-offer-further-options-at-no-cost-to-make-your-app-highly-available--these-options-include-inbuilt-load-balancing-autorecovery-of-unhealthy-container-instances-and-autoscaling-of-container-instances-based-on-cpu-and-memory-usage--map-a-public-route-to-your-container-group-to-make-your-app-accessible-from-the-internet----public-ip-addresses-use-these-endpoints-to-request-public-ip-addresses-for-your-space--you-can-bind-this-ip-address-to-your-container-to-make-your-container-accessible-from-the-internet---file-shares-create-list-and-delete-file-shares-in-a-space--a-file-share-is-a-nfs-storage-system-that-hosts-docker-volumes----volumes-create-and-manage-container-volumes-in-your-space-to-persist-the-data-of-your-containers----each-api-request-requires-an-http-header-that-includes-the-xauthtoken-and-xauthprojectid-parameter---xauthtoken-the-json-web-token-jwt-that-you-receive-when-logging-into-the-bluemix-platform--it-allows-you-to-use-the-ibm-containers-rest-api-access-services-and-resources--run-cf-oauthtoken-to-retrieve-your-access-token-information--xauthprojectid-the-unique-id-of-your-organization-space-where-you-want-to-create-or-work-with-your-containers--run-cf-space-space-name-guid-where-space-name-is-the-name-of-your-space-to-retrieve-your-space-id--for-further-information-about-how-containers-work-in-the-ibm-containers-service-review-the-documentation-under-httpsnewconsole-ng-bluemix-netdocscontainerscontainer-index-html--
  version: 3.0.0
host: containers-api.ng.bluemix.net
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /containers/groups:
    get:
      summary: List all container groups in a space
      description: 'This endpoint returns a list of all container groups in a space
        independent of their current state. (corresponding IBM Containers command:
        `cf ic group list`).'
      operationId: this-endpoint-returns-a-list-of-all-container-groups-in-a-space-independent-of-their-current-state--
      x-api-path-slug: containersgroups-get
      parameters:
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
    post:
      summary: Create and start a container group.
      description: "This endpoint creates and starts a new container group in your
        space. A container group consists of two or more single containers that are
        all created from the same container image and as a consequence are configured
        in the same way. Container groups offer different options at no cost to make
        your app highly available, such as in-built load balancing, auto-recovery
        of unhealthy container instances, and auto-scaling of container instances
        based on CPU and memory usage.\n\nTo create a container group with IBM Containers,
        you must at least define a container group name and the image that the container
        group is based on. Required attributes:\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n-
        Name: The container group name must start with a letter and then can include
        uppercase letters, lowercase letters, numbers, periods (.), underscores (_),
        or hyphens (-). \n- Image: You must include the full path to the image in
        your private Bluemix registry in the format:`registry.ng.bluemix.net/<namespace>/<image>`."
      operationId: this-endpoint-creates-and-starts-a-new-container-group-in-your-space--a-container-group-consists-of-
      x-api-path-slug: containersgroups-post
      parameters:
      - in: body
        name: RequiredAttributes
        description: Attributes that are required to create a container group in your
          space
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
  /containers/groups/{name_or_id}:
    delete:
      summary: Stop and delete all container instances in a container group.
      description: 'Stops and deletes the container instances that run in a container
        group (corresponding IBM Containers command: `cf ic group rm <group_name>`).
        When you delete a container group, all floating private IP addresses are released.'
      operationId: stops-and-deletes-the-container-instances-that-run-in-a-container-group-corresponding-ibm-containers
      x-api-path-slug: containersgroupsname-or-id-delete
      parameters:
      - in: query
        name: force
        description: If you want to force the deletion of a container group that has
          running container instances, use the force option
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          delete
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
    get:
      summary: Inspect a container group.
      description: 'This endpoint retrieves detailed information about a container
        group with a given name (corresponding IBM Containers command: `cf ic group
        inspect GROUP`).'
      operationId: this-endpoint-retrieves-detailed-information-about-a-container-group-with-a-given-name-corresponding
      x-api-path-slug: containersgroupsname-or-id-get
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          inspect
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
    patch:
      summary: Update a container group.
      description: "Update the number of container instances that run in a container
        group (corresponding IBM Containers command: `cf ic group update <option>
        <group>`). \n\nNote: You can run only one update at a time.  \n\n The desired
        number is the number of container instances that you require. It must be within
        the current limits of Max and Min. To increase the number of desired container
        instances above the Max value, you must first execute an update on the Max
        value. Once this update is completed, you can increase the desired number
        of container instances."
      operationId: update-the-number-of-container-instances-that-run-in-a-container-group-corresponding-ibm-containers-
      x-api-path-slug: containersgroupsname-or-id-patch
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group that you want to
          update
      - in: body
        name: Updates
        description: The container group parameter that you want to update
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
  /containers/groups/{name_or_id}/maproute:
    post:
      summary: Map a public route to a container group.
      description: 'If you want your container group to be accessible from the Internet,
        you need to expose a public port and map a public route to it (corresponding
        IBM Containers command: `cf ic route map -n <host> -d <domain> <group>`).
        Every route consists of the host name and domain.'
      operationId: if-you-want-your-container-group-to-be-accessible-from-the-internet-you-need-to-expose-a-public-port
      x-api-path-slug: containersgroupsname-or-idmaproute-post
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID of the container group to which you want
          to map a public route
      - in: body
        name: Route
        description: The public route that is mapped to the container group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
      - Maproute
  /containers/groups/{name_or_id}/unmaproute:
    post:
      summary: Unmap a public route from a container group
      description: "This endpoint unmaps a public route from a container group (corresponding
        IBM Containers command: `cf ic route unmap -n <host> -d <domain> <group>`).
        If no other public route is mapped to the container group, then the container
        group is no longer available from the internet. \n\n When you unmap a route
        from a container group, the route is not deleted and can be mapped to other
        container groups."
      operationId: this-endpoint-unmaps-a-public-route-from-a-container-group-corresponding-ibm-containers-command-cf-i
      x-api-path-slug: containersgroupsname-or-idunmaproute-post
      parameters:
      - in: path
        name: name_or_id
        description: The name or unique ID (UUID) of the container group that you
          want to inspect
      - in: body
        name: Route
        description: The public route that is unmapped from the container group
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Auth-Project-Id
        description: The unique ID of your organization space where you want to create
          or work with your containers
      - in: header
        name: X-Auth-Token
        description: The Bluemix JSON web token that you receive when logging into
          Bluemix
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Groups
      - Name
      - Unmaproute
---