---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid - Get Asm Groups
  x-api-slug: asmgroups-get
  description: |-
    **This endpoint allows you to retrieve information about multiple suppression groups.**

    This endpoint will return information for each group ID that you include in your request. To add a group ID to your request, simply append `&id=` followed by the group ID.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).

    Suppression groups, or [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html), allow you to label a category of content that you regularly send. This gives your recipients the ability to opt out of a specific set of your email. For example, you might define a group for your transactional email, and one for your marketing email so that your users can continue recieving your transactional email witout having to receive your marketing content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroups-get-openapi.md
- name: SendGrid - Add Asm Groups
  x-api-slug: asmgroups-post
  description: |-
    **This endpoint allows you to create a new suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroups-post-openapi.md
- name: SendGrid - Delete Asm Groups Group
  x-api-slug: asmgroupsgroup-id-delete
  description: |-
    **This endpoint allows you to delete a suppression group.**

    You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-delete-openapi.md
- name: SendGrid - Get Asm Groups Group
  x-api-slug: asmgroupsgroup-id-get
  description: |-
    **This endpoint allows you to retrieve a single suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-openapi.md
- name: SendGrid - Patch Asm Groups Group
  x-api-slug: asmgroupsgroup-id-patch
  description: |-
    **This endpoint allows you to update or change a suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-patch-openapi.md
- name: SendGrid - Get Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-get
  description: |-
    **This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-post
  description: |-
    **This endpoint allows you to add email addresses to an unsubscribe group.**

    If you attempt to add suppressions to a group that has been deleted or does not exist, the suppressions will be added to the global suppressions list.

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-post-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions Search
  x-api-slug: asmgroupsgroup-idsuppressionssearch-post
  description: |-
    **This endpoint allows you to search a suppression group for multiple suppressions.**

    When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionssearch-post-openapi.md
- name: SendGrid - Delete Asm Groups Group  Suppressions Email
  x-api-slug: asmgroupsgroup-idsuppressionsemail-delete
  description: |-
    **This endpoint allows you to remove a suppressed email address from the given suppression group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionsemail-delete-openapi.md
- name: SendGrid - Delete Asm Groups Group
  x-api-slug: asmgroupsgroup-id-delete
  description: |-
    **This endpoint allows you to delete a suppression group.**

    You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-delete-openapi.md
- name: SendGrid - Get Asm Groups Group
  x-api-slug: asmgroupsgroup-id-get
  description: |-
    **This endpoint allows you to retrieve a single suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-openapi.md
- name: SendGrid - Patch Asm Groups Group
  x-api-slug: asmgroupsgroup-id-patch
  description: |-
    **This endpoint allows you to update or change a suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-patch-openapi.md
- name: SendGrid - Get Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-get
  description: |-
    **This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-post
  description: |-
    **This endpoint allows you to add email addresses to an unsubscribe group.**

    If you attempt to add suppressions to a group that has been deleted or does not exist, the suppressions will be added to the global suppressions list.

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-post-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions Search
  x-api-slug: asmgroupsgroup-idsuppressionssearch-post
  description: |-
    **This endpoint allows you to search a suppression group for multiple suppressions.**

    When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionssearch-post-openapi.md
- name: SendGrid - Delete Asm Groups Group  Suppressions Email
  x-api-slug: asmgroupsgroup-idsuppressionsemail-delete
  description: |-
    **This endpoint allows you to remove a suppressed email address from the given suppression group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionsemail-delete-openapi.md
- name: SendGrid - Delete Asm Groups Group  Suppressions Email
  x-api-slug: asmgroupsgroup-idsuppressionsemail-delete
  description: |-
    **This endpoint allows you to remove a suppressed email address from the given suppression group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionsemail-delete-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions Search
  x-api-slug: asmgroupsgroup-idsuppressionssearch-post
  description: |-
    **This endpoint allows you to search a suppression group for multiple suppressions.**

    When given a list of email addresses and a group ID, this endpoint will return only the email addresses that have been unsubscribed from the given group.

    Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressionssearch-post-openapi.md
- name: SendGrid - Add Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-post
  description: |-
    **This endpoint allows you to add email addresses to an unsubscribe group.**

    If you attempt to add suppressions to a group that has been deleted or does not exist, the suppressions will be added to the global suppressions list.

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-post-openapi.md
- name: SendGrid - Get Asm Groups Group  Suppressions
  x-api-slug: asmgroupsgroup-idsuppressions-get
  description: |-
    **This endpoint allows you to retrieve all suppressed email addresses belonging to the given group.**

    Suppressions are recipient email addresses that are added to [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html). Once a recipient's address is on the suppressions list for an unsubscribe group, they will not receive any emails that are tagged with that unsubscribe group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-idsuppressions-get-openapi.md
- name: SendGrid - Patch Asm Groups Group
  x-api-slug: asmgroupsgroup-id-patch
  description: |-
    **This endpoint allows you to update or change a suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-patch-openapi.md
- name: SendGrid - Get Asm Groups Group
  x-api-slug: asmgroupsgroup-id-get
  description: |-
    **This endpoint allows you to retrieve a single suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-get-openapi.md
- name: SendGrid - Delete Asm Groups Group
  x-api-slug: asmgroupsgroup-id-delete
  description: |-
    **This endpoint allows you to delete a suppression group.**

    You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/sendgrid/asmgroupsgroup-id-delete-openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-api-gallery
  url: http://school.digger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sendgrid.stack.network
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---