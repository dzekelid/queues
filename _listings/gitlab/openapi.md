swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/sidekiq/queue_metrics:
    get:
      summary: Get Sekiq Queue Metrics
      description: Get the Sidekiq queue metrics
      operationId: getV3SidekiqQueueMetrics
      x-api-path-slug: v3sidekiqqueue-metrics-get
      responses:
        200:
          description: OK
      tags:
      - Sekiq
      - Queue
      - Metrics