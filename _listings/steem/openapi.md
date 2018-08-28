swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_miner_queue:
    get:
      summary: get_miner_queue
      description: get_miner_queue
      operationId: get-miner-queue
      x-api-path-slug: get-miner-queue-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Miner
      - Queue
  /get_liquidity_queue:
    get:
      summary: get_liquidity_queue
      description: get_liquidity_queue
      operationId: get-liquidity-queue
      x-api-path-slug: get-liquidity-queue-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: startAccount
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Liquidity
      - Queue