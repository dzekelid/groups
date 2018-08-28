---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Update a single modifier
  version: 1.0.0
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/item_groups:
    get:
      summary: Get all item groups
      description: |-
        Item Groups help merchants create and manage large groups of related items. This is described to merchants as an 'Item with variants'.

        For example a merchants may sell a t-shirt that is available in numerous various sizes and colors. Each of the t-shirt variations is an item and belongs to the t-shirt item group. Once an item group is created it appears in Register as a single button and tapping it brings up a choice of which variation is to be sold. Before adding items to an item group you first need to create the item group, then create attributes ('size', 'color') and then options for each attribute ('small', 'blue'), then associate options with an item and then associate items with an item group.

        The name of an item which is a member of an item group is automatically generated by the Clover server as a combination of the item group name and the name of all the options associated with that item. It cannot be changed. If the item group name is changed, or if an option name is changed, then the item names will be automatically regenerated.

        An item can only be a member of a single item group and once it is part of an item group it can never be removed or moved to another item group, it can only be deleted.
      operationId: GetItemGroups
      x-api-path-slug: v3merchantsmiditem-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, name, id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
    post:
      summary: Create an item group
      description: Create an item group.
      operationId: CreateItemGroup
      x-api-path-slug: v3merchantsmiditem-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
  /v3/merchants/{mId}/item_groups/{itemGroupId}:
    get:
      summary: Get a single item group
      description: Get a single item group.
      operationId: GetItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    post:
      summary: Update an item group
      description: Update an item group.
      operationId: UpdateItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items, attributes]'
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
    delete:
      summary: Delete an item group
      description: Delete an item group.
      operationId: DeleteItemGroup
      x-api-path-slug: v3merchantsmiditem-groupsitemgroupid-delete
      parameters:
      - in: path
        name: itemGroupId
        description: Item Group Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Groups
      - ItemGroupId
  /v3/merchants/{mId}/modifier_groups:
    get:
      summary: Get all modifier groups
      description: These groupings are the categories different modifiers belong to.
        Modifier groups can be made available for specific inventory Items by creating
        an item to modifier group association.
      operationId: GetModifierGroups
      x-api-path-slug: v3merchantsmidmodifier-groups-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
    post:
      summary: Create a modifier group
      description: Create a new modifier group. Modifiers can be associated with a
        modifier group after it has been created.
      operationId: CreateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
  /v3/merchants/{mId}/modifier_groups/{modGroupId}:
    get:
      summary: Get a modifier group
      description: Get a single modifier group by it's UUID
      operationId: GetModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    post:
      summary: Update a modifier group
      description: Update a modifier group. In order to add modifiers use the create
        modifiers endpoint.
      operationId: UpdateModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
    delete:
      summary: Delete a modifier group
      description: Delete an existing modifier group, identified by UUID. This also
        deletes all modifiers within that group.
      operationId: DeleteModifierGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
  /v3/merchants/{mId}/item_modifier_groups:
    post:
      summary: Create or delete item to modifier group associations
      description: 'Create or delete one or more association objects (item modifier
        groups). Modifiers can only be applied to items associated with that modifier''s
        group. Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
      operationId: CreateOrDeleteItemModifierGroups
      x-api-path-slug: v3merchantsmiditem-modifier-groups-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Modifier
      - Groups
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers:
    get:
      summary: Get all modifiers belonging to a single modifier group
      description: Get an array containing the modifiers in a single modifier group.
      operationId: GetModifiersByGroup
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifiers, items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, price, name, alternateName, id,
          modifierGroup'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
    post:
      summary: Create a modifier
      description: Create a modifier object belonging to the modifier group identified
        in the URL.
      operationId: CreateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
  /v3/merchants/{mId}/modifier_groups/{modGroupId}/modifiers/{modId}:
    get:
      summary: Get a single modifier
      description: Get a single modifier by it's group, and it's UUID
      operationId: GetModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
    post:
      summary: Update a single modifier
      description: Update a modifier. Note that once it has been created, it is not
        possible to change a modifier's group.
      operationId: UpdateModifier
      x-api-path-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [modifierGroup]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modGroupId
        description: Modifier Group Id
      - in: path
        name: modId
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Groups
      - ModGroupId
      - Modifiers
      - ModId
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