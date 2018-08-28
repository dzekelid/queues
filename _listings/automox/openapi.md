swagger: "2.0"
x-collection-name: Automox
x-complete: 1
info:
  title: Automox API
  description: the-automox-api-is-a-powerful-interface-that-allows-you-to-integrate-automox-reporting-data-into-you-applications-and-control-the-various-settings-of-your-account-all-endpoints-are-only-accessible-via-https-and-are-located-atapi-automox-com--for-instance-you-can-see-events-associated-with-your-account-by-accessing-the-following-url-with-your-idreplace-apikey-with-your-own--httpsconsole-automox-comapieventsapi-keyapikey-limitsbe-nice--if-youre-sending-too-many-requests-too-quickly-well-send-back-a429-error-code-too-many-requests-you-are-limited-to-5000-requests-per-hour-per-api-key-overall--practically-this-means-you-should-when-possible-authenticateusers-so-that-limits-are-well-outside-the-reach-of-a-given-user-
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers/{id}/queues:
    get:
      summary: Get Servers Queues
      description: Returns the command queue for the specified server (endpoint)
      operationId: returns-the-command-queue-for-the-specified-server-endpoint
      x-api-path-slug: serversidqueues-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
    post:
      summary: Post Servers Queues
      description: Issue a command to an endpoint. Can be used to install a specific
        set of patches or reboot an endpoint
      operationId: issue-a-command-to-an-endpoint-can-be-used-to-install-a-specific-set-of-patches-or-reboot-an-endpoin
      x-api-path-slug: serversidqueues-post
      parameters:
      - in: body
        name: command
        description: Command object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
  /users/{id}/queues:
    get:
      summary: Get Users Queues
      description: Gets all commands executed for specified user id
      operationId: gets-all-commands-executed-for-specified-user-id
      x-api-path-slug: usersidqueues-get
      parameters:
      - in: path
        name: id
        description: User ID or `self` for current user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Queues