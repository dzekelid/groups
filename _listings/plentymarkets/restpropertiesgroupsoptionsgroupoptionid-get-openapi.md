---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a group option
  description: Gets a group option. The ID of the group option must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/property_groups:
    get:
      summary: List property groups
      description: Lists the property groups.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-get
      parameters:
      - in: query
        name: with
        description: Includes the specified property group information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-post
      parameters:
      - in: body
        name: /rest/items/property_groups
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups:
    get:
      summary: List property groups
      description: Lists property groups.
      operationId: getRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-get
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
    post:
      summary: Create a property group
      description: Creates a property group.
      operationId: postRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-post
      parameters:
      - in: body
        name: /rest/properties/groups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/accounts/contacts/group_functions:
    get:
      summary: List all group function related data
      description: Lists all data that is related to the contact group function contents.
      operationId: getRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Group
      - Function
      - Related
      - Data
    post:
      summary: Apply selected group function options for given contact IDs
      description: Applies selected group function options for given contact IDs.
      operationId: postRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-post
      parameters:
      - in: query
        name: addressLabelTemplate
        description: An address label template ID
      - in: query
        name: contactList
        description: A list of contact IDs
      - in: query
        name: emailTemplate
        description: An email template ID
      - in: query
        name: newsletter
        description: A newsletter folder ID
      responses:
        200:
          description: OK
      tags:
      - Apply
      - Selected
      - Group
      - Function
      - Optionsgiven
      - Contact
      - IDs
  /rest/items/property_groups/{id}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates an existing property group.
      operationId: putRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groupsid-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/items/property_groups/{id}/names:
    get:
      summary: List the property group names of a property group
      description: Lists the property group names of a property group in all languages.
        The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Group
      - Names
      - Of
      - Property
      - Group
    post:
      summary: Create a property group name
      description: Creates a property group name. The ID of the property group must
        be specified.
      operationId: postRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-post
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/items/property_groups/{id}/names/{lang}:
    delete:
      summary: Delete a property group name
      description: Deletes a property group name. The ID of the property group must
        be specified.
      operationId: deleteRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
    get:
      summary: Get a property group name in a language
      description: Gets a property group name in the specified language. The ID of
        the property group name and the language code must be specified.
      operationId: getRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
      - In
      - Language
    put:
      summary: Update a property group name
      description: Updates a property group name. The ID of the property group and
        the language must be specified.
      operationId: putRestItemsPropertyGroupsNamesLang
      x-api-path-slug: restitemsproperty-groupsidnameslang-put
      parameters:
      - in: body
        name: /rest/items/property_groups/{id}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
      - Name
  /rest/properties/groups/names:
    get:
      summary: List group names
      description: Lists group names.
      operationId: getRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Names
    post:
      summary: Create an group name
      description: Create an group name.
      operationId: postRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-post
      parameters:
      - in: body
        name: /rest/properties/groups/names
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: lang
        description: The lang of the group name
      - in: query
        name: name
        description: The name of the group name
      - in: query
        name: propertyId
        description: The ID of the property
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
  /rest/properties/groups/names/{groupNameId}:
    delete:
      summary: Delete a group name
      description: Deletes a group name. The ID of the group name must be specified.
      operationId: deleteRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-delete
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
    get:
      summary: Get a group name
      description: Gets a group name. The ID of the group name must be specified.
      operationId: getRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-get
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
    put:
      summary: Update a group name
      description: Updates a group name. The ID of the group name must be specified.
      operationId: putRestPropertiesGroupsNamesGroupname
      x-api-path-slug: restpropertiesgroupsnamesgroupnameid-put
      parameters:
      - in: path
        name: groupNameId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Name
  /rest/properties/groups/options:
    get:
      summary: List group options
      description: Lists group options.
      operationId: getRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Options
    post:
      summary: Create a group option
      description: Creates a group option
      operationId: postRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-post
      parameters:
      - in: body
        name: /rest/properties/groups/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: groupOptionIdentifier
        description: The groupOptionIdentifier of the group name
      - in: query
        name: propertyGroupId
        description: The ID of the property group
      - in: query
        name: value
        description: The value of the group name
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/groups/options/{groupOptionId}:
    delete:
      summary: Delete a group option
      description: Deletes a group option. The ID of the group option must be specified.
      operationId: deleteRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-delete
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    get:
      summary: Get a group option
      description: Gets a group option. The ID of the group option must be specified.
      operationId: getRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-get
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    put:
      summary: Update a group option
      description: Updates a group option. The ID of the group option must be specified.
      operationId: putRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-put
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/groups/types:
    get:
      summary: Get group types from module configuration
      description: Get group types from module configuration.
      operationId: getRestPropertiesGroupsTypes
      x-api-path-slug: restpropertiesgroupstypes-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Types
      - From
      - Module
      - Configuration
  /rest/properties/groups/{groupId}:
    get:
      summary: Get a property group
      description: Gets a property group. The ID of the property group must be specified.
      operationId: getRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-get
      parameters:
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
    put:
      summary: Update a property group
      description: Updates a property group. The ID of the property group must be
        specified.
      operationId: putRestPropertiesGroupsGroup
      x-api-path-slug: restpropertiesgroupsgroupid-put
      parameters:
      - in: body
        name: /rest/properties/groups/{groupId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
      - in: query
        name: names
        description: The names of the group
      - in: query
        name: options
        description: The options of the group
      - in: query
        name: position
        description: The position  of the group
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/properties/groups/{groupId}/properties/{propertyId}:
    delete:
      summary: Detach a property from a property group.
      description: Detaches a property from a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: deleteRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-delete
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Detach
      - Property
      - From
      - Property
      - Group
    post:
      summary: Attach a property to a property group
      description: Attaches a property to a property group. The ID of the property
        and the ID of the property group must be specified.
      operationId: postRestPropertiesGroupsGroupPropertiesProperty
      x-api-path-slug: restpropertiesgroupsgroupidpropertiespropertyid-post
      parameters:
      - in: path
        name: groupId
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Attach
      - Property
      - To
      - Property
      - Group
  /rest/properties/groups/{propertyId}:
    delete:
      summary: Delete a property group
      description: Deletes a property group. The ID of the property group must be
        specified.
      operationId: deleteRestPropertiesGroupsProperty
      x-api-path-slug: restpropertiesgroupspropertyid-delete
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Group
  /rest/warehouses/locations/group:
    put:
      summary: Edit the purpose and status for a group of storage locations
      description: Edits the purpose and status for a group of storage locations by
        passing the group storage location ID (can be sent as mass assignment)
      operationId: putRestWarehousesLocationsGroup
      x-api-path-slug: restwarehouseslocationsgroup-put
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Purpose
      - Statusa
      - Group
      - Of
      - Storage
      - Locations
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