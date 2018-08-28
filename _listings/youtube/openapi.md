swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    delete:
      summary: Delete Groups
      description: Deletes a group.
      operationId: deleteGroups
      x-api-path-slug: groups-delete
      parameters:
      - in: query
        name: id
        description: The id parameter specifies the YouTube group ID for the group
          that is being deleted
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    get:
      summary: Get Groups
      description: Returns a collection of groups that match the API request parameters.
        For example, you can retrieve all groups that the authenticated user owns,
        or you can retrieve one or more groups by their unique IDs.
      operationId: getGroups
      x-api-path-slug: groups-get
      parameters:
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          group ID(s) for the resource(s) that are being retrieved
      - in: query
        name: mine
        description: Set this parameters value to true to instruct the API to only
          return groups owned by the authenticated user
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: pageToken
        description: The pageToken parameter identifies a specific page in the result
          set that should be returned
      responses:
        200:
          description: OK
      tags:
      - Groups
    post:
      summary: Add Groups
      description: Creates a group.
      operationId: postGroups
      x-api-path-slug: groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups
    put:
      summary: Put Groups
      description: Modifies a group. For example, you could change a group's title.
      operationId: putGroups
      x-api-path-slug: groups-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      responses:
        200:
          description: OK
      tags:
      - Groups