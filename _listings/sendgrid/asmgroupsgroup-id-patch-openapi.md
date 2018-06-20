---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Patch Asm Groups Group
  description: |-
    **This endpoint allows you to update or change a suppression group.**

    Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

    The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

    Each user can create up to 25 different suppression groups.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /asm/groups:
    get:
      summary: Get Asm Groups
      description: |-
        **This endpoint allows you to retrieve information about multiple suppression groups.**

        This endpoint will return information for each group ID that you include in your request. To add a group ID to your request, simply append `&id=` followed by the group ID.

        Suppressions are a list of email addresses that will not receive content sent under a given [group](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html).

        Suppression groups, or [unsubscribe groups](https://sendgrid.com/docs/API_Reference/Web_API_v3/Suppression_Management/groups.html), allow you to label a category of content that you regularly send. This gives your recipients the ability to opt out of a specific set of your email. For example, you might define a group for your transactional email, and one for your marketing email so that your users can continue recieving your transactional email witout having to receive your marketing content.
      operationId: asm.groups.get
      x-api-path-slug: asmgroups-get
      parameters:
      - in: query
        name: id
        description: The ID of a suppression group that you want to retrieve information
          for
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
    post:
      summary: Add Asm Groups
      description: |-
        **This endpoint allows you to create a new suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.post
      x-api-path-slug: asmgroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
  /asm/groups/{group_id}:
    delete:
      summary: Delete Asm Groups Group
      description: |-
        **This endpoint allows you to delete a suppression group.**

        You can only delete groups that have not been attached to sent mail in the last 60 days. If a recipient uses the "one-click unsubscribe" option on an email associated with a deleted group, that recipient will be added to the global suppression list.

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.delete
      x-api-path-slug: asmgroupsgroup-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
    get:
      summary: Get Asm Groups Group
      description: |-
        **This endpoint allows you to retrieve a single suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.get
      x-api-path-slug: asmgroupsgroup-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
    patch:
      summary: Patch Asm Groups Group
      description: |-
        **This endpoint allows you to update or change a suppression group.**

        Suppression groups, or unsubscribe groups, are specific types or categories of email that you would like your recipients to be able to unsubscribe from. For example: Daily Newsletters, Invoices, System Alerts.

        The **name** and **description** of the unsubscribe group will be visible by recipients when they are managing their subscriptions.

        Each user can create up to 25 different suppression groups.
      operationId: asm.groups.group_id.patch
      x-api-path-slug: asmgroupsgroup-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Asm
      - Groups
      - Group
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