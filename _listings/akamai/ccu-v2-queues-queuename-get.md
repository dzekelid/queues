---
swagger: "2.0"
info:
  title: Akamai API Get Current Queue Size
  description: Get Current Queue Size
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ccu/v2/queues/{queueName}:
    get:
      summary: Get Current Queue Size
      description: Get Current Queue Size
      operationId: ccuv2queuesqueuename
      parameters:
      - in: query
        name: queueName
        description: Name of the queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - ccu
      - queues
      - queues
definitions: []
x-collection-name: Akamai
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