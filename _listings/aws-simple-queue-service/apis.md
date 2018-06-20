---
name: AWS Simple Queue Service
x-slug: aws-simple-queue-service
description: Amazon Simple Queue Service (SQS) is a fast, reliable, scalable, fully
  managed message queuing service. Amazon SQS makes it simple and cost-effective to
  decouple the components of a cloud application. You can use Amazon SQS to transmit
  any volume of data, without losing messages or requiring other services to be always
  available. Amazon SQS includesstandard queueswith high throughput and at-least-once
  processing, andFIFO queuesthat provide FIFO (first-in, first-out) delivery and exactly-once
  processing. With Amazon SQS, you can offload the administrative burden of operating
  and scaling a highly available messaging cluster, while paying a low price for only
  what you use.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Queues
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Queue Service API Create Queue
  x-api-slug: aws-simple-queue-service-api
  description: Creates a new standard or FIFO queue or returns the URL of an existing
    queue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=CreateQueue
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actioncreatequeue-get-openapi.md
- name: AWS Simple Queue Service API Delete Queue
  x-api-slug: aws-simple-queue-service-api
  description: Deletes the queue specified by the QueueUrl, even if the queue is empty.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=DeleteQueue
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actiondeletequeue-get-openapi.md
- name: AWS Simple Queue Service API Get Queue Attributes
  x-api-slug: aws-simple-queue-service-api
  description: Gets attributes for the specified queue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=GetQueueAttributes
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actiongetqueueattributes-get-openapi.md
- name: AWS Simple Queue Service API Get Queue Url
  x-api-slug: aws-simple-queue-service-api
  description: Returns the URL of an existing queue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=GetQueueUrl
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actiongetqueueurl-get-openapi.md
- name: AWS Simple Queue Service API List Dead Letter Source Queues
  x-api-slug: aws-simple-queue-service-api
  description: Returns a list of your queues that have the RedrivePolicy queue attribute
    configured with a dead letter queue.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=ListDeadLetterSourceQueues
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actionlistdeadlettersourcequeues-get-openapi.md
- name: AWS Simple Queue Service API List Queues
  x-api-slug: aws-simple-queue-service-api
  description: Returns a list of your queues.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=ListQueues
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actionlistqueues-get-openapi.md
- name: AWS Simple Queue Service API Purge Queue
  x-api-slug: aws-simple-queue-service-api
  description: Deletes the messages in a queue specified by the QueueURL parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=PurgeQueue
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actionpurgequeue-get-openapi.md
- name: AWS Simple Queue Service API Set Queue Attributes
  x-api-slug: aws-simple-queue-service-api
  description: Sets the value of one or more queue attributes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: ://///?Action=SetQueueAttributes
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/actionsetqueueattributes-get-openapi.md
- name: AWS Simple Queue Service API
  x-api-slug: aws-simple-queue-service-api
  description: Amazon Simple Queue Service (SQS) is a fast, reliable, scalable, fully
    managed message queuing service. Amazon SQS makes it simple and cost-effective
    to decouple the components of a cloud application. You can use Amazon SQS to transmit
    any volume of data, without losing messages or requiring other services to be
    always available. Amazon SQS includesstandard queueswith high throughput and at-least-once
    processing, andFIFO queuesthat provide FIFO (first-in, first-out) delivery and
    exactly-once processing. With Amazon SQS, you can offload the administrative burden
    of operating and scaling a highly available messaging cluster, while paying a
    low price for only what you use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Application-Services_AmazonSQS.png
  humanURL: https://aws.amazon.com/sqs/
  baseURL: :///
  tags: Queues
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/queues/master/_listings/aws-simple-queue-service/openapi.md
x-common:
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SQ
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sqs/index.html
- type: x-console
  url: https://console.aws.amazon.com/sqs/
- type: x-documentation
  url: http://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/sqs/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=12
- type: x-getting-started
  url: https://aws.amazon.com/sqs/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/sqs/pricing/
- type: x-website
  url: https://aws.amazon.com/sqs/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---