---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Post Ticket Groups Ticket Group
  description: Updates the ticket group with the specified :ticket_group_id. Returns
    the updated ticket_group.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/:event_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Groups
      description: |-
        Get the list of ticket_group for the event with the specified :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketGroups
      x-api-path-slug: eventsevent-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Groups
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/:
    post:
      summary: Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Add the Ticket Class with the specified :ticket_class_id that belongs
        to the event with :event_id to the Ticket Group identified by :ticket_group_id.
      operationId: postEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
    delete:
      summary: Delete Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Remove the Ticket Class with the specified :ticket_class_id that
        belongs to the event with :event_id from the Ticket Group identified by :ticket_group_id.
      operationId: deleteEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
  /ticket_groups/:ticket_group_id/:
    get:
      summary: Get Ticket Groups Ticket Group
      description: Returns the ticket_group with the specified :ticket_group_id.
      operationId: getTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-get
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
    delete:
      summary: Delete Ticket Groups Ticket Group
      description: |-
        Deletes the ticket_group with the specified :ticket_group_id.
        The status of the ticket group is changed to deleted.
      operationId: deleteTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-delete
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
    post:
      summary: Post Ticket Groups Ticket Group
      description: Updates the ticket group with the specified :ticket_group_id. Returns
        the updated ticket_group.
      operationId: postTicketGroupsTicketGroup
      x-api-path-slug: ticket-groupsticket-group-id-post
      parameters:
      - in: query
        name: ticket_group.event_ticket_ids
        description: (&#8216;IDs of tickets by event id for this ticket group
        type: query
      - in: query
        name: ticket_group.name
        description: Name of ticket group
        type: query
      - in: query
        name: ticket_group.status
        description: The status of ticket group
        type: query
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
      - :ticket
      - Group
  /ticket_groups/:
    post:
      summary: Post Ticket Groups
      description: |-
        Creates a ticket group and returns the created ticket_group.
        Only up to 200 live ticket groups may be created; those with archived or deleted status are not taken into account.
      operationId: postTicketGroups
      x-api-path-slug: ticket-groups-post
      parameters:
      - in: query
        name: ticket_group.event_ticket_ids
        description: (&#8216;IDs of tickets by event id for this ticket group
        type: query
      - in: query
        name: ticket_group.name
        description: Name of ticket group
        type: query
      - in: query
        name: ticket_group.status
        description: The status of ticket group
        type: query
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Groups
  /users/:user_id/ticket_groups/:
    get:
      summary: Get Users User Ticket Groups
      description: |-
        Returns a paginated response of ticket_group for the specified user.
        The alias me (/users/me/) may be used to refer to the currently authenticated user.
      operationId: getUsersUserTicketGroups
      x-api-path-slug: usersuser-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Ticket
      - Groups
  /users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    post:
      summary: Post Users User Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
        belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
        If the list provided is empty, remove this ticket class from every ticket group.
      operationId: postUsersUserEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
      parameters:
      - in: query
        name: ticket_group_ids
        description: IDs of all ticket group this ticket belongs to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
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