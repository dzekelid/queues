swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/call-queues:
    get:
      summary: Get Call Queues
      description: |-
        Returns call queue group list
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Medium
      operationId: listCallQueues
      x-api-path-slug: restapiv1-0accountaccountidcallqueues-get
      parameters:
      - in: path
        name: accountId
      - in: query
        name: memberExtensionId
        description: Internal identifier of an extension that is a member of every
          group within the result
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Queues
  /restapi/v1.0/account/{accountId}/department/bulk-assign:
    post:
      summary: Edit Call Queue Members
      description: "[Deprecated] Adds and/or removes multiple call queue members\nApp
        Permission\nEditAccounts\nUser Permission\nUserGroups\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nEXT-401\nExtension
        ID should be present only in one section"
      operationId: bulkAssignDepartments
      x-api-path-slug: restapiv1-0accountaccountiddepartmentbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Call
      - Queue
      - Members
  /restapi/v1.0/account/{accountId}/call-queues/{groupId}/members:
    get:
      summary: Get Call Queue Members
      description: |-
        Returns call queue group members.
        App Permission
        ReadAccounts
        User Permission
        ReadExtensions
        Usage Plan Group
        Light
      operationId: listCallQueueMembers
      x-api-path-slug: restapiv1-0accountaccountidcallqueuesgroupidmembers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: groupId
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Queue
      - Members
  /restapi/v1.0/account/{accountId}/call-queues/{groupId}/bulk-assign:
    post:
      summary: Edit Call Queue Group
      description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser
        Permission\nGroups\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n400\nEXT-405\nExtension of
        type [ParkLocation] could not be a member of [department}]"
      operationId: updateCallQueueGroup
      x-api-path-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
      parameters:
      - in: path
        name: accountId
      - in: body
        name: body
        description: Changes for the given group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Call
      - Queue
      - Group