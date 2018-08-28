swagger: "2.0"
x-collection-name: AWS Batch
x-complete: 1
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeJobQueues:
    get:
      summary: Describe Job Queues
      description: Describes one or more of your job queues.
      operationId: describeJobQueues
      x-api-path-slug: actiondescribejobqueues-get
      parameters:
      - in: query
        name: jobQueues
        description: A list of up to 100 queue names or full queue Amazon Resource
          Name (ARN) entries
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results returned by DescribeJobQueues in
          paginated         output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated            DescribeJobQueues
          request where maxResults was used and the         results exceeded the value
          of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Queue
  /?Action=CreateJobQueue:
    get:
      summary: Create Job Queue
      description: Creates an AWS Batch job queue.
      operationId: createJobQueue
      x-api-path-slug: actioncreatejobqueue-get
      parameters:
      - in: query
        name: computeEnvironmentOrder
        description: The set of compute environments mapped to a job queue and their
          order relative to         each other
        type: string
      - in: query
        name: jobQueueName
        description: The name of the job queue
        type: string
      - in: query
        name: priority
        description: The priority of the job queue
        type: string
      - in: query
        name: state
        description: The state of the job queue
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Queue
  /?Action=DeleteJobQueue:
    get:
      summary: Delete Job Queue
      description: Deletes the specified job queue.
      operationId: deleteJobQueue
      x-api-path-slug: actiondeletejobqueue-get
      parameters:
      - in: query
        name: jobQueue
        description: The short name or full Amazon Resource Name (ARN) of the queue
          to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Queue
  /?Action=UpdateJobQueue:
    get:
      summary: Update Job Queue
      description: Updates a job queue.
      operationId: updateJobQueue
      x-api-path-slug: actionupdatejobqueue-get
      parameters:
      - in: query
        name: computeEnvironmentOrder
        description: Details the set of compute environments mapped to a job queue
          and their order         relative to each other
        type: string
      - in: query
        name: jobQueue
        description: The name or the Amazon Resource Name (ARN) of the job queue
        type: string
      - in: query
        name: priority
        description: The priority of the job queue
        type: string
      - in: query
        name: state
        description: Describes the queues ability to accept new jobs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Queue