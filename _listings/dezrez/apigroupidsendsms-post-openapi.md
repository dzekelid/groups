---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez To send an adhoc sms to a group
  version: 1.0.0
  description: To send an adhoc sms to a group.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/setbranch:
    post:
      summary: Set the Groups home Branch
      description: Set the groups home branch.
      operationId: Group_SetBranchByidBysetBranchCommand
      x-api-path-slug: apigroupidsetbranch-post
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setBranchCommand
        description: The set branch data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Groups
      - Home
      - Branch
  /api/group/{id}/setteam:
    post:
      summary: Set the Groups owning team
      description: Set the groups owning team.
      operationId: Group_SetOwningTeamByidBysetTeamCommand
      x-api-path-slug: apigroupidsetteam-post
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setTeamCommand
        description: The set owning team data contract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Groups
      - Owning
      - Team
  /api/group/updateprimarygroupmember:
    put:
      summary: Return the Groups with appointments between a given date range, ordered
        by appointments Count
      description: Return the groups with appointments between a given date range,
        ordered by appointments count.
      operationId: Group_UpdatePrimaryGroupMemberByfilter
      x-api-path-slug: apigroupupdateprimarygroupmember-put
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Appointments
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Appointments
      - Count
  /api/group/mostactive:
    get:
      summary: Return the Groups with the most viewings between a given date range,
        ordered by viewing Count
      description: Return the groups with the most viewings between a given date range,
        ordered by viewing count.
      operationId: Group_MostActiveBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.roleTypes
      x-api-path-slug: apigroupmostactive-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Groups
      - Most
      - Viewings
      - Between
      - Given
      - Date
      - Range
      - ""
      - Ordered
      - By
      - Viewing
      - Count
  /api/group/geoaggregation/{zoom}:
    post:
      summary: Returns GeoAggregations of all searching groups
      description: Returns geoaggregations of all searching groups.
      operationId: Group_GeoAggregationByzoom
      x-api-path-slug: apigroupgeoaggregationzoom-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: zoom
      responses:
        200:
          description: OK
      tags:
      - Returns
      - GeoAggregations
      - Of
      - ""
      - Searching
      - Groups
  /api/group/{id}/setflags:
    put:
      summary: Sets the interest flags on groups interest role.
      description: Sets the interest flags on groups interest role..
      operationId: Group_SetInterestFlagsByidByflagsDataContract
      x-api-path-slug: apigroupidsetflags-put
      parameters:
      - in: body
        name: flagsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Interest
      - Flags
      - "On"
      - Groups
      - Interest
      - Role
  /api/group/archivegroups:
    post:
      summary: Archive groups in bulk
      description: Archive groups in bulk.
      operationId: Group_ArchiveGroupsBydeleteCommand
      x-api-path-slug: apigrouparchivegroups-post
      parameters:
      - in: body
        name: deleteCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Archive
      - Groups
      - In
      - Bulk
  /api/list/groups/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupFilterByid
      x-api-path-slug: apilistgroupsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/list/groupinterests:
    post:
      summary: Get list of groups and what they are interested in.
      description: Get list of groups and what they are interested in..
      operationId: List_GroupInterestsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistgroupinterests-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - What
      - They
      - Are
      - Interested
      - In
  /api/list/groupinterests/groupinterestidsfiltered:
    post:
      summary: Get list of groups and what they are interested in.
      description: Get list of groups and what they are interested in..
      operationId: List_GetInterestsFilteredByfilter
      x-api-path-slug: apilistgroupinterestsgroupinterestidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - What
      - They
      - Are
      - Interested
      - In
  /api/list/groupinterests/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupInterestListFilterByid
      x-api-path-slug: apilistgroupinterestsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/negotiator/my/groups/favourite:
    get:
      summary: Returns a list of the logged in negotiators favourite groups.
      description: Returns a list of the logged in negotiators favourite groups..
      operationId: Negotiator_FavouriteGroupsBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormygroupsfavourite-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Logged
      - In
      - Negotiators
      - Favourite
      - Groups
  /api/role/{id}/matches:
    get:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidBypageSizeBypageNumberByadjustedAskingPriceBysortByminScore
      x-api-path-slug: apiroleidmatches-get
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: minScore
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
    post:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidByfilterBypageSizeBypageNumberByadjustedAskingPriceBysort
      x-api-path-slug: apiroleidmatches-post
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
  /api/teamsecurity/permissionsforgroup:
    get:
      summary: This returns security permissions that a group has on other groups
      description: This returns security permissions that a group has on other groups.
      operationId: TeamGroupSecurity_GetSecurityPermissionsForGroupByteamId
      x-api-path-slug: apiteamsecuritypermissionsforgroup-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: The id of the group to find permissions for
      responses:
        200:
          description: OK
      tags:
      - This
      - Returns
      - Security
      - Permissions
      - That
      - Group
      - Has
      - "On"
      - Other
      - Groups
  /api/teamsecurity/permissionsongroup:
    get:
      summary: This returns security permissions that other groups have on specified
        group
      description: This returns security permissions that other groups have on specified
        group.
      operationId: TeamGroupSecurity_GetSecurityPermissionsThatApplyToGroupByteamId
      x-api-path-slug: apiteamsecuritypermissionsongroup-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: The id of the group to find other groups permissions
      responses:
        200:
          description: OK
      tags:
      - This
      - Returns
      - Security
      - Permissions
      - That
      - Other
      - Groups
      - Have
      - "On"
      - Specified
      - Group
  /api/globalsearch/groups:
    get:
      summary: Search for Groups across the system.
      description: Search for groups across the system..
      operationId: GlobalSearch_GroupsBydataContract.termBydataContract.pageSizeBydataContract.pageNumberBydataContract
      x-api-path-slug: apiglobalsearchgroups-get
      parameters:
      - in: query
        name: dataContract.branchId
      - in: query
        name: dataContract.excludeArchived
      - in: query
        name: dataContract.excludeDeleted
      - in: query
        name: dataContract.groupTypes
      - in: query
        name: dataContract.lastUpdated
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.serviceType
      - in: query
        name: dataContract.term
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - SearchGroups
      - Across
      - System
  /api/customfieldgroup/{typeName}:
    get:
      summary: Get a list of custom field groups for a type and optional group name
        specified.
      description: Get a list of custom field groups for a type and optional group
        name specified..
      operationId: CustomFieldGroup_GetBytypeNameBygroupName
      x-api-path-slug: apicustomfieldgrouptypename-get
      parameters:
      - in: query
        name: groupName
        description: An optional parameter to filter by group name
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: typeName
        description: The name of the type to get the custom field groups for
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Custom
      - Field
      - Groupsa
      - Type
      - Optional
      - Group
      - Name
      - Specified
  /api/documentgeneration/previewpack:
    post:
      summary: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack
      description: Generates a pack using the first selected group/property of a type
        to get a quick preview of the pack.
      operationId: DocumentGeneration_PreviewPackByrandomPackDataContract
      x-api-path-slug: apidocumentgenerationpreviewpack-post
      parameters:
      - in: body
        name: randomPackDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Pack
      - Using
      - First
      - Selected
      - Group
      - Property
      - Of
      - Type
      - To
      - Get
      - Quick
      - Preview
      - Of
      - Pack
  /api/documentgeneration/vendorreport:
    post:
      summary: Generates a correspondence to a single group, sending them a single
        report for multiple properties
      description: Generates a correspondence to a single group, sending them a single
        report for multiple properties.
      operationId: DocumentGeneration_SendVendorReportBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorreport-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Group
      - ""
      - Sending
      - Them
      - Single
      - Reportmultiple
      - Properties
  /api/group/{id}:
    get:
      summary: Get a group by its Id
      description: Get a group by its id.
      operationId: Group_GetByid
      x-api-path-slug: apigroupid-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Group
      - By
      - Its
      - Id
  /api/group/delete:
    post:
      summary: Delete a group
      description: Delete a group.
      operationId: Group_DeleteBydeleteCommand
      x-api-path-slug: apigroupdelete-post
      parameters:
      - in: body
        name: deleteCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Group
  /api/group/{id}/deletegroupmember:
    delete:
      summary: Delete a contact from a group
      description: Delete a contact from a group.
      operationId: Group_DeleteGroupMemberByidBydeleteCommand
      x-api-path-slug: apigroupiddeletegroupmember-delete
      parameters:
      - in: body
        name: deleteCommand
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Contact
      - From
      - Group
  /api/group/addgroup:
    post:
      summary: Adds a Group
      description: Adds a group.
      operationId: Group_AddGroupBygroupSaveCommandDataContract
      x-api-path-slug: apigroupaddgroup-post
      parameters:
      - in: body
        name: groupSaveCommandDataContract
        description: A wrapper for the group save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Group
  /api/group/{id}/addgroupmember:
    put:
      summary: Add a new contact to an existing group
      description: Add a new contact to an existing group.
      operationId: Group_AddGroupMemberByidByaddGroupMemberDataContract
      x-api-path-slug: apigroupidaddgroupmember-put
      parameters:
      - in: body
        name: addGroupMemberDataContract
        description: The details of the person
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - New
      - Contact
      - To
      - Existing
      - Group
  /api/group/{id}/savesalessearch:
    post:
      summary: Saves Search Criteria to a Group
      description: Saves search criteria to a group.
      operationId: Group_SaveSalesSearchByidBysearchDataContract
      x-api-path-slug: apigroupidsavesalessearch-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchDataContract
        description: The groups search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Search
      - Criteria
      - To
      - Group
  /api/group/{id}/savelettingssearch:
    post:
      summary: Saves Lettings Search Criteria to a group
      description: Saves lettings search criteria to a group.
      operationId: Group_SaveLettingsSearchByidBysearchingDataContract
      x-api-path-slug: apigroupidsavelettingssearch-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchingDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Lettings
      - Search
      - Criteria
      - To
      - Group
  /api/group/{id}/deletesearch/{searchingRoleId}:
    delete:
      summary: Deletes Search Criteria from a Group
      description: Deletes search criteria from a group.
      operationId: Group_DeleteSearchByidBysearchingRoleId
      x-api-path-slug: apigroupiddeletesearchsearchingroleid-delete
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: searchingRoleId
        description: The id of the searching role to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Search
      - Criteria
      - From
      - Group
  /api/group/{id}/salessearching:
    get:
      summary: Get Sales Searching Roles for a Group
      description: Get sales searching roles for a group.
      operationId: Group_SearchingSalesRolesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidsalessearching-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Searching
      - Rolesa
      - Group
  /api/group/{id}/lettingssearching:
    get:
      summary: Get Lettings Searching Roles for a Group
      description: Get lettings searching roles for a group.
      operationId: Group_SearchingLettingsRolesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidlettingssearching-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lettings
      - Searching
      - Rolesa
      - Group
  /api/group/{id}/searching/{roleId}/matches:
    get:
      summary: Get property matches for a Searching Role for a Group
      description: Get property matches for a searching role for a group.
      operationId: Group_PropertyMatchesByidByroleIdBypageSizeBypageNumberBysort
      x-api-path-slug: apigroupidsearchingroleidmatches-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      - in: query
        name: sort
      responses:
        200:
          description: OK
      tags:
      - Property
      - Matchesa
      - Searching
      - Rolea
      - Group
    post:
      summary: Get property matches for a Searching Role for a Group
      description: Get property matches for a searching role for a group.
      operationId: Group_PropertyMatchesByidByroleIdByfilterBypageSizeBypageNumberBysort
      x-api-path-slug: apigroupidsearchingroleidmatches-post
      parameters:
      - in: body
        name: filter
        description: Match filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Group Id
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Amount of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: Role Id
      - in: query
        name: sort
        description: How to sort the results
      responses:
        200:
          description: OK
      tags:
      - Property
      - Matchesa
      - Searching
      - Rolea
      - Group
  /api/group/{id}/events:
    get:
      summary: Get group events by its Id
      description: Get group events by its id.
      operationId: Group_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryTypeByactiveRolesOnly
      x-api-path-slug: apigroupidevents-get
      parameters:
      - in: query
        name: activeRolesOnly
        description: Only return active roles
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: excludedTypes
        description: Bring back all except these types
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the group to get events for
      - in: query
        name: includeDrafts
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: query
        name: propertyId
        description: The property the event must relate to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Events
      - By
      - Its
      - Id
  /api/group/{id}/displaysettings:
    put:
      summary: Edit Display settings for the Group. Primarily shown in the GroupHub
        e.g. the icon and background image.
      description: Edit display settings for the group. primarily shown in the grouphub
        e.g. the icon and background image..
      operationId: Group_SetDisplaySettingsByidBygroupDisplaySettingsDataContract
      x-api-path-slug: apigroupiddisplaysettings-put
      parameters:
      - in: body
        name: groupDisplaySettingsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Display
      - Settingsthe
      - Group
      - ""
      - Primarily
      - Shown
      - In
      - GroupHub
      - E
      - G
      - ""
      - Icon
      - Background
      - Image
  /api/group/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a group
      description: Attaches an existing document to a group.
      operationId: Group_AttachDocumentByidBydocumentId
      x-api-path-slug: apigroupidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the group to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Group
  /api/group/{id}/detachdocument:
    put:
      summary: Detaches a document from a group
      description: Detaches a document from a group.
      operationId: Group_DetachDocumentByidBydocumentId
      x-api-path-slug: apigroupiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the group to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Group
  /api/group/{id}/uploadandattachdocument:
    post:
      summary: Uploads a new document and attaches it to the specified group.
      description: Uploads a new document and attaches it to the specified group..
      operationId: Group_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apigroupiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Document
      - Attaches
      - It
      - To
      - Specified
      - Group
  /api/group/{id}/setdescription:
    put:
      summary: Sets the description of the specified group
      description: Sets the description of the specified group.
      operationId: Group_SetDescriptionByidBynewDescriptionCommand
      x-api-path-slug: apigroupidsetdescription-put
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: body
        name: newDescriptionCommand
        description: The set description data contract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Description
      - Of
      - Specified
      - Group
  /api/group/{id}/documents:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc
      x-api-path-slug: apigroupiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: orderDesc
        description: Order by created date descending (true by default)
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/made:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersMadeByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersmade-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/received:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersReceivedByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersreceived-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/properties:
    get:
      summary: Return a list of properties that the group owns
      description: Return a list of properties that the group owns.
      operationId: Group_GroupPropertiesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidproperties-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Properties
      - That
      - Group
      - Owns
  /api/group/{id}/saveadditionalinfo:
    put:
      summary: To save or edit the Group additional info i.e. the Origin and Grade.
      description: To save or edit the group additional info i.e. the origin and grade..
      operationId: Group_SaveAdditionalInfoByidBysaveAdditionalInfoDataContract
      x-api-path-slug: apigroupidsaveadditionalinfo-put
      parameters:
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: saveAdditionalInfoDataContract
        description: The additional info to set on the group i
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Save
      - Edit
      - Group
      - Additional
      - Info
      - I
      - E
      - ""
      - Origin
      - Grade
  /api/group/{id}/saveadditionalquestions:
    put:
      summary: To edit the Group additional questions
      description: To edit the group additional questions.
      operationId: Group_SaveAdditionalQuestionsByidByadditionalQuestions
      x-api-path-slug: apigroupidsaveadditionalquestions-put
      parameters:
      - in: body
        name: additionalQuestions
        description: The additional questions to set on the group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Edit
      - Group
      - Additional
      - Questions
  /api/group/{id}/sendemail:
    post:
      summary: To send an adhoc email to a group
      description: To send an adhoc email to a group.
      operationId: Group_SendEmailByidByemailDataContract
      x-api-path-slug: apigroupidsendemail-post
      parameters:
      - in: body
        name: emailDataContract
        description: Details of the email to send
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Email
      - To
      - Group
  /api/group/{id}/sendsms:
    post:
      summary: To send an adhoc sms to a group
      description: To send an adhoc sms to a group.
      operationId: Group_SendSMSByidBysmsDataContract
      x-api-path-slug: apigroupidsendsms-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: smsDataContract
        description: Details of the sms to send
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Send
      - Adhoc
      - Sms
      - To
      - Group
  /api/group/setgroupmembersorder:
    put:
      summary: Sets order for members of a group
      description: Sets order for members of a group.
      operationId: Group_SetGroupMembersOrderBygroupMembersOrderDataContract
      x-api-path-slug: apigroupsetgroupmembersorder-put
      parameters:
      - in: body
        name: groupMembersOrderDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Ordermembers
      - Of
      - Group
  /api/group/{id}/roles:
    get:
      summary: Get the roles for a Group by Group id
      description: Get the roles for a group by group id.
      operationId: Group_RolesByidBypageSizeBypageNumberByroleTypesByroleStatuses
      x-api-path-slug: apigroupidroles-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get the roles for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleStatuses
      - in: query
        name: roleTypes
      responses:
        200:
          description: OK
      tags:
      - Rolesa
      - Group
      - By
      - Group
      - Id
  /api/group/recordcontact:
    post:
      summary: Records an event on the group representing a neg being in contact
      description: Records an event on the group representing a neg being in contact.
      operationId: Group_RecordContactByrecordGroupContactDataContract
      x-api-path-slug: apigrouprecordcontact-post
      parameters:
      - in: body
        name: recordGroupContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Group
      - Representing
      - Neg
      - Being
      - In
      - Contact
  /api/group/{id}/undelete:
    put:
      summary: Undelete a group
      description: Undelete a group.
      operationId: Group_SetStatusByidByunDeleteGroupDataContract
      x-api-path-slug: apigroupidundelete-put
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: unDeleteGroupDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Undelete
      - Group
  /api/group/{id}/addpreferredcompany:
    post:
      summary: Add a preferred company to a group
      description: Add a preferred company to a group.
      operationId: Group_AddPreferredCompanyByidBycompanyIdBypreferredContactId
      x-api-path-slug: apigroupidaddpreferredcompany-post
      parameters:
      - in: query
        name: companyId
      - in: path
        name: id
      - in: query
        name: preferredContactId
        description: The person id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Preferred
      - Company
      - To
      - Group
  /api/group/{id}/removepreferredcompany:
    post:
      summary: Remove a preferred company to a group
      description: Remove a preferred company to a group.
      operationId: Group_RemovePreferredCompanyByidBycompanyId
      x-api-path-slug: apigroupidremovepreferredcompany-post
      parameters:
      - in: query
        name: companyId
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Preferred
      - Company
      - To
      - Group
  /api/todo/group/savetodo:
    post:
      summary: Saves or Updates a Group ToDo and its tasks
      description: Saves or updates a group todo and its tasks.
      operationId: GroupToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodogroupsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - S
      - Group
      - ToDo
      - Its
      - Tasks
  /api/todo/group/addtasks:
    put:
      summary: Add task to a Group ToDo
      description: Add task to a group todo.
      operationId: GroupToDo_AddTasksByaddTasksCommandDataContract
      x-api-path-slug: apitodogroupaddtasks-put
      parameters:
      - in: body
        name: addTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Task
      - To
      - Group
      - ToDo
  /api/todo/group/getupcomingtask:
    get:
      summary: Get the todo and latest task for a group
      description: Get the todo and latest task for a group.
      operationId: GroupToDo_GetUpComingTaskBygroupId
      x-api-path-slug: apitodogroupgetupcomingtask-get
      parameters:
      - in: query
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Todo
      - Latest
      - Taska
      - Group
  /api/inboundlead/{todoTaskLeadId}/setleadgroup/{groupId}:
    put:
      summary: Endpoint to update group on inbound lead task
      description: Endpoint to update group on inbound lead task.
      operationId: InboundLead_SetLeadGroupBytodoTaskLeadIdBygroupId
      x-api-path-slug: apiinboundleadtodotaskleadidsetleadgroupgroupid-put
      parameters:
      - in: path
        name: groupId
        description: Group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: todoTaskLeadId
        description: Todos Task Id
      responses:
        200:
          description: OK
      tags:
      - Endpoint
      - To
      - Update
      - Group
      - "On"
      - Inbound
      - Lead
      - Task
  /api/progression/lettings/addguarantor:
    put:
      summary: Add Guarantor to the letting group.
      description: Add guarantor to the letting group..
      operationId: LettingsProgression_AddGuarantorByaddGuarantorDataContractBytenantRoleIdBygroupId
      x-api-path-slug: apiprogressionlettingsaddguarantor-put
      parameters:
      - in: body
        name: addGuarantorDataContract
        description: The details of the person
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: groupId
        description: The id for guarantor if guarantor person in multiple groups
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantRoleId
        description: The id of the tenant role
      responses:
        200:
          description: OK
      tags:
      - Guarantor
      - To
      - Letting
      - Group
  /api/progression/lettings/uploadandattachguarantorgroupdocument:
    post:
      summary: Allows you to upload a lettings document and attach it directly to
        a guarantor group.
      description: Allows you to upload a lettings document and attach it directly
        to a guarantor group..
      operationId: LettingsProgression_UploadAndAttachGurantorGroupDocumentByguarantorGroupIdBytenancyIdBydocumentDetai
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantorgroupdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorGroupId
        description: The guarantor group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenancyId
        description: The tenancy Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Lettings
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
      - Group
  /api/progression/lettings/removeguarantor:
    put:
      summary: Add Guarantor to the letting group.
      description: Add guarantor to the letting group..
      operationId: LettingsProgression_RemoveGuarantorBytenantRoleIdByguarantorGroupId
      x-api-path-slug: apiprogressionlettingsremoveguarantor-put
      parameters:
      - in: query
        name: guarantorGroupId
        description: The group id of the guarantor
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantRoleId
        description: The id of the tenant role
      responses:
        200:
          description: OK
      tags:
      - Guarantor
      - To
      - Letting
      - Group
  /api/progression/lettings/removeguarantors:
    put:
      summary: Add Guarantor to the letting group.
      description: Add guarantor to the letting group..
      operationId: LettingsProgression_RemoveGuarantorsBytenantRoleIdBydataContract
      x-api-path-slug: apiprogressionlettingsremoveguarantors-put
      parameters:
      - in: body
        name: dataContract
        description: The guarantor IDS to remove
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantRoleId
        description: The id of the tenant role
      responses:
        200:
          description: OK
      tags:
      - Guarantor
      - To
      - Letting
      - Group
  /api/list/groups/groupidsfiltered:
    post:
      summary: Get list of group ids
      description: Get list of group ids.
      operationId: List_GetGroupListFilteredByfilter
      x-api-path-slug: apilistgroupsgroupidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Group
      - Ids
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
  /api/list/activesearches/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateActiveSearchCsvBycommandDataContract
      x-api-path-slug: apilistactivesearchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupmatches/csv:
    post:
      summary: Generates a csv file from group matches by property role id
      description: Generates a csv file from group matches by property role id.
      operationId: List_GenerateGroupMatchesCsvBycommandDataContract
      x-api-path-slug: apilistgroupmatchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Group
      - Matches
      - By
      - Property
      - Role
      - Id
  /api/list/propertyfinancial/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateFinancialPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertyfinancialcsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/followups:
    post:
      summary: Gets a list of group followups
      description: Gets a list of group followups.
      operationId: List_FollowUpsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistfollowups-post
      parameters:
      - in: body
        name: filter
        description: Filter for follow ups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size, limited to 100
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Group
      - Followups
  /api/list/feedback/followups:
    post:
      summary: Gets a list of group followups
      description: Gets a list of group followups.
      operationId: List_FeedbackFollowUpsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistfeedbackfollowups-post
      parameters:
      - in: body
        name: filter
        description: Filter for follow ups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size, limited to 100
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Group
      - Followups
  /api/negotiator/my/groups/favourite/add/{groupId}:
    post:
      summary: Add a favourite group to the negotiators list of favourites.
      description: Add a favourite group to the negotiators list of favourites..
      operationId: Negotiator_AddFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteaddgroupid-post
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Favourite
      - Group
      - To
      - Negotiators
      - List
      - Of
      - Favourites
  /api/negotiator/my/groups/favourite/remove/{groupId}:
    delete:
      summary: Remove a group from a Negotiators favourite list.
      description: Remove a group from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteremovegroupid-delete
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Negotiators
      - Favourite
      - List
  /api/property/{id}/addgrouptoproperty:
    put:
      summary: Creates/Adds a group to the CurrentOwners of the supplied PropertyId
      description: Creates/adds a group to the currentowners of the supplied propertyid.
      operationId: Property_AddGroupToPropertyByidBydatacontract
      x-api-path-slug: apipropertyidaddgrouptoproperty-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Group
      - To
      - CurrentOwners
      - Of
      - Supplied
      - PropertyId
  /api/receipt/addfunds:
    post:
      summary: Add funds to an account/group by id or suspense account
      description: Add funds to an account/group by id or suspense account.
      operationId: Receipt_ReceiptFundsByreceiptFundsDataContract
      x-api-path-slug: apireceiptaddfunds-post
      parameters:
      - in: body
        name: receiptFundsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Funds
      - To
      - Account
      - Group
      - By
      - Id
      - Suspense
      - Account
  /api/role/{id}/addgrouptopropertyrole:
    put:
      summary: Creates/Adds a group to the supplied roleId
      description: Creates/adds a group to the supplied roleid.
      operationId: Role_AddGroupToPropertyRoleByidBydatacontract
      x-api-path-slug: apiroleidaddgrouptopropertyrole-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Group
      - To
      - Supplied
      - RoleId
  /api/teamsecurity/savepermission:
    post:
      summary: Save a new security permission for a group
      description: Save a new security permission for a group.
      operationId: TeamGroupSecurity_SavePermissionBydataContract
      x-api-path-slug: apiteamsecuritysavepermission-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - New
      - Security
      - Permissiona
      - Group
  /api/teams/{id}/setteamresponsibilities:
    put:
      summary: Sets the responsibilties for a team group
      description: Sets the responsibilties for a team group.
      operationId: Teams_SetTeamResponsibilitiesByidByresponsibities
      x-api-path-slug: apiteamsidsetteamresponsibilities-put
      parameters:
      - in: path
        name: id
      - in: body
        name: responsibities
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Responsibiltiesa
      - Team
      - Group
  /api/group/{id}/notes:
    get:
      summary: Get notes for Group
      description: Get notes for group.
      operationId: Group_NotesByidBypinnedBypageNumberBypageSize
      x-api-path-slug: apigroupidnotes-get
      parameters:
      - in: path
        name: id
        description: Group Id
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: query
        name: pinned
        description: Only show pinned notes
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - NotesGroup
  /api/group/{id}/setsearchteam:
    post:
      summary: Set the Team Group for a searching role
      description: Set the team group for a searching role.
      operationId: Group_SetSearchTeamByidBysetTeamCommandDataContract
      x-api-path-slug: apigroupidsetsearchteam-post
      parameters:
      - in: path
        name: id
        description: Group that owns the searching role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setTeamCommandDataContract
        description: Set Team Group Command
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Team
      - Groupa
      - Searching
      - Role
  /api/property/{id}/owners:
    get:
      summary: For a given property, will return owning PeopleGroup
      description: For a given property, will return owning peoplegroup.
      operationId: Property_OwnersByid
      x-api-path-slug: apipropertyidowners-get
      parameters:
      - in: path
        name: id
        description: property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - For
      - Given
      - Property
      - ""
      - Will
      - Return
      - Owning
      - PeopleGroup
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