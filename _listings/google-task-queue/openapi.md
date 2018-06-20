---
swagger: "2.0"
x-collection-name: Google Task Queue
x-complete: 1
info:
  title: TaskQueue
  description: accesses-a-google-app-engine-pull-task-queue-over-rest-
  contact:
    name: Google
    url: https://google.com
  version: v1beta2
host: www.googleapis.com
basePath: /taskqueue/v1beta2/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/taskqueues/{taskqueue}:
    get:
      summary: Get Task Queues
      description: Get detailed information about a TaskQueue.
      operationId: taskqueue.taskqueues.get
      x-api-path-slug: projecttaskqueuestaskqueue-get
      parameters:
      - in: query
        name: getStats
        description: Whether to get stats
      - in: path
        name: project
        description: The project under which the queue lies
      - in: path
        name: taskqueue
        description: The id of the taskqueue to get the properties of
      responses:
        200:
          description: OK
      tags:
      - Task Queues
---