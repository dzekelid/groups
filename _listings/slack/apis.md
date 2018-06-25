---
name: Slack
x-slug: slack
description: Slack is a team communication application providing services such as
  real-time messaging, archiving, and to search for modern teams. It offers one-on-one
  messaging, private groups, persistent chat rooms, and direct messaging as well as
  group chats organized by topic. All content inside Slack is searchable from one
  search box and it integrates with a number of third-party services, including Google
  Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Groups
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/apis.md
specificationVersion: "0.14"
apis:
- name: Slack Get Group Thread
  x-api-slug: slack
  description: Retrieve a thread of messages posted to a private channel
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.replies
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-replies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-replies-get-openapi.md
- name: Slack Rename Group
  x-api-slug: slack
  description: Renames a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.rename
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-rename-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-rename-post-openapi.md
- name: Slack Get Group
  x-api-slug: slack
  description: Lists private channels that the calling user has access to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.list
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-list-get-openapi.md
- name: Slack Remove User From Group
  x-api-slug: slack
  description: Removes a user from a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.kick
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-kick-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-kick-post-openapi.md
- name: Slack Mark Group
  x-api-slug: slack
  description: Sets the read cursor in a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.mark
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-mark-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-mark-post-openapi.md
- name: Slack List Group Users
  x-api-slug: slack
  description: List all users in a User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.users.list
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-users-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-users-list-get-openapi.md
- name: Slack Get Group
  x-api-slug: slack
  description: Gets information about a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.info
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-info-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-info-get-openapi.md
- name: Slack Update Group Users
  x-api-slug: slack
  description: Update the list of users for a User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.users.update
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-users-update-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-users-update-post-openapi.md
- name: Slack Update Group
  x-api-slug: slack
  description: Update an existing User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.update
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-update-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-update-post-openapi.md
- name: Slack Leave Group
  x-api-slug: slack
  description: Leaves a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.leave
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-leave-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-leave-post-openapi.md
- name: Slack Create Group
  x-api-slug: slack
  description: Create a User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.create
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-create-post-openapi.md
- name: Slack Create Child Group
  x-api-slug: slack
  description: Clones and archives a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.createChild
  tags: Messaging,Groups, archives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-createchild-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-createchild-post-openapi.md
- name: Slack Enable Group
  x-api-slug: slack
  description: Enable a User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.enable
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-enable-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-enable-post-openapi.md
- name: Slack Invite User To Group
  x-api-slug: slack
  description: Invites a user to a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.invite
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-invite-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-invite-post-openapi.md
- name: Slack Create Group
  x-api-slug: slack
  description: Creates a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.create
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-create-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-create-post-openapi.md
- name: Slack List Groups
  x-api-slug: slack
  description: List all User Groups for a team
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.list
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-list-get-openapi.md
- name: Slack Open Group
  x-api-slug: slack
  description: Opens a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.open
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-open-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-open-post-openapi.md
- name: Slack Group History
  x-api-slug: slack
  description: Fetches history of messages and events from a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.history
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-history-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-history-get-openapi.md
- name: Slack Set Group Topic
  x-api-slug: slack
  description: Sets the topic for a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.setTopic
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-settopic-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-settopic-post-openapi.md
- name: Slack Disable Group
  x-api-slug: slack
  description: Disable an existing User Group
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//usergroups.disable
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-disable-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/usergroups-disable-post-openapi.md
- name: Slack Set Group Purpose
  x-api-slug: slack
  description: Sets the purpose for a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.setPurpose
  tags: Messaging,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-setpurpose-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-setpurpose-post-openapi.md
- name: Slack Unarchive Group
  x-api-slug: slack
  description: Unarchives a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.unarchive
  tags: Messaging,Groups, Archives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-unarchive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-unarchive-post-openapi.md
- name: Slack Archive Group
  x-api-slug: slack
  description: Archives a private channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api//groups.archive
  tags: Messaging,Groups,Archives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-archive-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/groups-archive-post-openapi.md
- name: Slack
  x-api-slug: slack
  description: Slack is a team communication application providing services such as
    real-time messaging, archiving, and to search for modern teams. It offers one-on-one
    messaging, private groups, persistent chat rooms, and direct messaging as well
    as group chats organized by topic. All content inside Slack is searchable from
    one search box and it integrates with a number of third-party services, including
    Google Docs, Dropbox, Heroku, Crashlytics, GitHub, and Zendesk.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/slack-logo.png
  humanURL: https://api.slack.com
  baseURL: https://slack.com//api
  tags: Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/slack/openapi.md
x-common:
- type: x-website
  url: https://api.slack.com
- type: x-application-gallery
  url: https://slack.com/apps
- type: x-blog
  url: http://slackhq.com/
- type: x-blog
  url: https://medium.com/slack-developer-blog
- type: x-blog-rss
  url: http://slackhq.com/rss
- type: x-blog-rss
  url: https://medium.com/feed/slack-developer-blog
- type: x-branding
  url: https://slack.com/brand-guidelines
- type: x-buttons
  url: https://api.slack.com/docs/slack-button
- type: x-c-sharp-sdk
  url: https://api.slack.com/web
- type: x-change-log
  url: https://api.slack.com/changelog
- type: x-developer
  url: https://api.slack.com/
- type: x-faq
  url: https://api.slack.com/faq
- type: x-getting-started
  url: https://slack.com/getting-started
- type: x-github
  url: https://github.com/slackhq
- type: x-incoming-webhooks
  url: https://api.slack.com/incoming-webhooks
- type: x-oauth-overview
  url: https://api.slack.com/docs/oauth
- type: x-oauth-scopes
  url: https://api.slack.com/docs/oauth-scopes
- type: x-outgoing-webhooks
  url: https://api.slack.com/outgoing-webhooks
- type: x-presence
  url: https://api.slack.com/docs/presence
- type: x-pricing
  url: https://slack.com/pricing
- type: x-privacy
  url: https://slack.com/privacy-policy
- type: x-rate-limits
  url: https://api.slack.com/docs/rate-limits
- type: x-real-time-messaging-api
  url: https://api.slack.com/rtm
- type: x-road-map
  url: https://api.slack.com/roadmap
- type: x-security
  url: https://slack.com/security
- type: x-status
  url: https://status.slack.com/
- type: x-support
  url: https://get.slack.help/hc/en-us
- type: x-terms-of-service
  url: https://slack.com/terms-of-service
- type: x-transparency-report
  url: https://slack.com/transparency-report
- type: x-twitter
  url: https://twitter.com/slackapi
- type: x-website
  url: http://slack.com
- type: x-website
  url: https://slack.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---