---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Groups Pools Get Photos
  description: Returns a list of pool photos for a given group, based on the permissions
    of the group and the user logged in (if any).
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.groups.browse:
    get:
      summary: Groups Browse
      description: Browse the group category tree, finding groups and sub-categories.
      operationId: getRestMethodFlickr.groups.browse
      x-api-path-slug: restmethodflickr-groups-browse-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: cat_id
        description: The category id to fetch a list of groups and sub-categories
          for
      - in: query
        name: format
        description: Response format
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Browse
  /rest/?method=flickr.groups.getInfo:
    get:
      summary: Groups Get Info
      description: Get information about a group.
      operationId: getRestMethodFlickr.groups.getinfo
      x-api-path-slug: restmethodflickr-groups-getinfo-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: group_id
        description: The NSID of the group to fetch information for
      - in: query
        name: lang
        description: The language of the group name and description to fetch
      responses:
        200:
          description: OK
      tags:
      - Groups
      - GetInfo
  /rest/?method=flickr.groups.search:
    get:
      summary: Groups Search
      description: Search for groups. 18+ groups will only be returned for authenticated
        calls where the authenticated user is over 18.
      operationId: getRestMethodFlickr.groups.search
      x-api-path-slug: restmethodflickr-groups-search-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of groups to return per page
      - in: query
        name: text
        description: The text to search for
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Search
  /rest/?method=flickr.groups.members.getList:
    get:
      summary: Groups Members Get List
      description: Get a list of the members of a group. The call must be signed on
        behalf of a Flickr member, and the ability to see the group membership will
        be determined by the Flickr member's group privileges.
      operationId: getRestMethodFlickr.groups.members.getlist
      x-api-path-slug: restmethodflickr-groups-members-getlist-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: group_id
        description: Return a list of members for this group
      - in: query
        name: membertypes
        description: Comma separated list of member types
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of groups to return per page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Members
      - GetList
  /rest/?method=flickr.groups.pools.add:
    post:
      summary: Groups Pools Add
      description: Add a photo to a group's pool.
      operationId: postRestMethodFlickr.groups.pools.add
      x-api-path-slug: restmethodflickr-groups-pools-add-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: group_id
        description: The NSID of the group whose pool the photo is to be added to
      - in: query
        name: photo_id
        description: The id of the photo to add to the group pool
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - Add
  /rest/?method=flickr.groups.pools.getContext:
    get:
      summary: Groups Pools Get Context
      description: Returns next and previous photos for a photo in a group pool.
      operationId: getRestMethodFlickr.groups.pools.getcontext
      x-api-path-slug: restmethodflickr-groups-pools-getcontext-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: group_id
        description: The NSID of the group whose pool to fetch the photos context
          for
      - in: query
        name: photo_id
        description: The id of the photo to fetch the context for
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - GetContext
  /rest/?method=flickr.groups.pools.getGroups:
    get:
      summary: Groups Pools Get Groups
      description: Returns a list of groups to which you can add photos.
      operationId: getRestMethodFlickr.groups.pools.getgroups
      x-api-path-slug: restmethodflickr-groups-pools-getgroups-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of groups to return per page
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - GetGroups
  /rest/?method=flickr.groups.pools.getPhotos:
    get:
      summary: Groups Pools Get Photos
      description: Returns a list of pool photos for a given group, based on the permissions
        of the group and the user logged in (if any).
      operationId: getRestMethodFlickr.groups.pools.getphotos
      x-api-path-slug: restmethodflickr-groups-pools-getphotos-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: extras
        description: A comma-delimited list of extra information to fetch for each
          returned record
      - in: query
        name: format
        description: Response format
      - in: query
        name: page
        description: The page of results to return
      - in: query
        name: per_page
        description: Number of photos to return per page
      - in: query
        name: tags
        description: A tag to filter the pool with
      - in: query
        name: user_id
        description: The nsid of a user
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Pools
      - GetPhotos
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---