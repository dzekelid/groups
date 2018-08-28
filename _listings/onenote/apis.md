---
name: OneNote
x-slug: onenote
description: Microsoft OneNote (formerly called Microsoft Office OneNote) is a computer
  program for free-form information gathering and multi-user collaboration. It gathers
  users notes (handwritten or typed), drawings, screen clippings and audio commentaries.
  Notes can be shared with other OneNote users over the Internet or a network. OneNote
  is available as a part of the Microsoft Office suite. It is also available as a
  free stand-alone application for Windows, Mac, Windows RT, Windows Phone, iOS, Android
  and Symbian.[4] A web-based version of OneNote is provided as part of OneDrive or
  Office Online and enables users to edit notes via a web browser.
image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
x-kinRank: "7"
x-alexaRank: "5531"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/apis.md
specificationVersion: "0.14"
apis:
- name: One Note Get Sectiongroups Sectiongroupid Sectiongroups
  x-api-slug: one-note
  description: Returns a collection of section groups within a specific section group.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sectionGroups
  tags: SectionGroups,SectionGroupId,SectionGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-get-openapi.md
- name: One Note Parameters Sectiongroups Sectiongroupid Sectiongroups
  x-api-slug: one-note
  description: Parameters sectiongroups sectiongroupid sectiongroups.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sectionGroups
  tags: SectionGroups,SectionGroupId,SectionGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-parameters-openapi.md
- name: One Note Get Sectiongroups Sectiongroupid Sections
  x-api-slug: one-note
  description: Returns a collection of sections within a specific section group.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sections
  tags: SectionGroups,SectionGroupId,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-get-openapi.md
- name: One Note Parameters Sectiongroups Sectiongroupid Sections
  x-api-slug: one-note
  description: Parameters sectiongroups sectiongroupid sections.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sections
  tags: SectionGroups,SectionGroupId,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-parameters-openapi.md
- name: One Note Get Sectiongroups Sectiongroupid
  x-api-slug: one-note
  description: Returns a specific section group object.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}
  tags: SectionGroups,SectionGroupId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupid-get-openapi.md
- name: One Note Parameters Sectiongroups Sectiongroupid
  x-api-slug: one-note
  description: Parameters sectiongroups sectiongroupid.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}
  tags: SectionGroups,SectionGroupId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupid-parameters-openapi.md
- name: One Note Get Sectiongroups
  x-api-slug: one-note
  description: Returns a collection of section groups.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/
  tags: SectionGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroups-get-openapi.md
- name: One Note Parameters Sectiongroups
  x-api-slug: one-note
  description: Parameters sectiongroups.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/
  tags: SectionGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroups-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroups-parameters-openapi.md
- name: One Note Get Notebooks Notebookid Sectiongroups
  x-api-slug: one-note
  description: Returns a collection of section groups within a specific notebook.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///notebooks/{notebookId}/sectiongroups
  tags: Notebooks,NotebookId,Sectiongroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-get-openapi.md
- name: One Note Parameters Notebooks Notebookid Sectiongroups
  x-api-slug: one-note
  description: Parameters notebooks notebookid sectiongroups.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///notebooks/{notebookId}/sectiongroups
  tags: Notebooks,NotebookId,Sectiongroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-parameters-openapi.md
- name: One Note Post Notebooks Notebookid Sectiongroups
  x-api-slug: one-note
  description: Creates a new section group in a notebook.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///notebooks/{notebookId}/sectiongroups
  tags: Notebooks,NotebookId,Sectiongroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/notebooksnotebookidsectiongroups-post-openapi.md
- name: One Note Post Sectiongroups Sectiongroupid Sections
  x-api-slug: one-note
  description: Post sectiongroups sectiongroupid sections.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sections
  tags: SectionGroups,SectionGroupId,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsections-post-openapi.md
- name: One Note Post Sectiongroups Sectiongroupid Sectiongroups
  x-api-slug: one-note
  description: Post sectiongroups sectiongroupid sectiongroups.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes///sectionGroups/{sectionGroupId}/sectionGroups
  tags: SectionGroups,SectionGroupId,SectionGroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/sectiongroupssectiongroupidsectiongroups-post-openapi.md
- name: One Note
  x-api-slug: one-note
  description: Microsoft OneNote (formerly called Microsoft Office OneNote) is a computer
    program for free-form information gathering and multi-user collaboration. It gathers
    users notes (handwritten or typed), drawings, screen clippings and audio commentaries.
    Notes can be shared with other OneNote users over the Internet or a network. OneNote
    is available as a part of the Microsoft Office suite. It is also available as
    a free stand-alone application for Windows, Mac, Windows RT, Windows Phone, iOS,
    Android and Symbian.[4] A web-based version of OneNote is provided as part of
    OneDrive or Office Online and enables users to edit notes via a web browser.
  image: https://s3.amazonaws.com/kinlane-productions/api-evangelist/api-butterfly.png
  humanURL: http://onenote.com
  baseURL: https://www.onenote.com//api/v1.0/me/notes/
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/onenote/openapi.md
x-common:
- type: x-application-gallery
  url: http://dev.office.com/showcase
- type: x-blog
  url: http://blogs.msdn.com/b/onenotedev/
- type: x-blog-rss
  url: http://blogs.msdn.com/b/onenotedev/rss.aspx
- type: x-console
  url: https://apigee.com/onenote/embed/console/onenote
- type: x-developer
  url: http://dev.onenote.com/
- type: x-getting-started
  url: http://msdn.microsoft.com/en-us/library/office/dn575425.aspx
- type: x-github
  url: https://github.com/OneNoteDev
- type: x-twitter
  url: https://twitter.com/OneNoteDev
- type: x-privacy
  url: http://go.microsoft.com/fwlink/?LinkId=391953&clcid=0x409
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/onenote
- type: x-terms-of-service
  url: http://go.microsoft.com/fwlink/?LinkId=391954&clcid=0x409
- type: x-trademarks
  url: http://go.microsoft.com/fwlink/p/?LinkId=316970
- type: x-website
  url: http://onenote.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---