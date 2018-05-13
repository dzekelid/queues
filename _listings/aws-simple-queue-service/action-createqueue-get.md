---
swagger: "2.0"
info:
  title: AWS Simple Queue Service API Create Queue
  version: 1.0.0
  description: Creates a new standard or FIFO queue or returns the URL of an existing
    queue.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateQueue:
    get:
      summary: ' Create Queue '
      description: Creates a new standard or FIFO queue or returns the URL of an existing
        queue
      operationId: createQueue
      parameters:
      - in: query
        name: |-
          Attribute
                      , Attribute.N.Name (key), Attribute.N.Value (value)
        description: A map of attributes with their corresponding values
        type: string
      - in: query
        name: QueueName
        description: The name of the new queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - queues
definitions: []
x-collection-name: AWS Simple Queue Service
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