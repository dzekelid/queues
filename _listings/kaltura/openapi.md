---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/batch/action/getQueueSize:
    get:
      summary: Get Service Batch Action Getqueuesize
      description: batch getQueueSize action get the queue size for job type
      operationId: batch.getQueueSize
      x-api-path-slug: servicebatchactiongetqueuesize-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: workerQueueFilter[filter][advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoriesMatchOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoryEntryStatusIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][categoryIdEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentLike]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentMultiLikeAnd]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][contentMultiLikeOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointsFreeText]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][cuePointTypeIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][depthGreaterThanEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][distributionProfileId]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: workerQueueFilter[filter][advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][extendedStatusIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][field]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][idEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][idIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][indexIdGreaterThan]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][items]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberIdEq]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberIdIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][metadataProfileId]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][noDistributionProfiles]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][not]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][objectType]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: workerQueueFilter[filter][advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][userIdEqual]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][userIdIn]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][value]
      - in: query
        name: workerQueueFilter[filter][advancedSearch][watermarkId]
      - in: query
        name: workerQueueFilter[filter][batchVersionEqual]
      - in: query
        name: workerQueueFilter[filter][batchVersionGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][batchVersionLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][createdAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][createdAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][entryIdEqual]
      - in: query
        name: workerQueueFilter[filter][errNumberEqual]
      - in: query
        name: workerQueueFilter[filter][errNumberIn]
      - in: query
        name: workerQueueFilter[filter][errNumberNotIn]
      - in: query
        name: workerQueueFilter[filter][errTypeEqual]
        description: 'Enum Type: `KalturaBatchJobErrorTypes`'
      - in: query
        name: workerQueueFilter[filter][errTypeIn]
      - in: query
        name: workerQueueFilter[filter][errTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][estimatedEffortGreaterThan]
      - in: query
        name: workerQueueFilter[filter][estimatedEffortLessThan]
      - in: query
        name: workerQueueFilter[filter][executionAttemptsGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][executionAttemptsLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][finishTimeGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][finishTimeLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][idEqual]
      - in: query
        name: workerQueueFilter[filter][idGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeEqual]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobSubTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeAndSubTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeEqual]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: workerQueueFilter[filter][jobTypeIn]
      - in: query
        name: workerQueueFilter[filter][jobTypeNotIn]
      - in: query
        name: workerQueueFilter[filter][lockVersionGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][lockVersionLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][objectType]
      - in: query
        name: workerQueueFilter[filter][orderBy]
      - in: query
        name: workerQueueFilter[filter][partnerIdEqual]
      - in: query
        name: workerQueueFilter[filter][partnerIdIn]
      - in: query
        name: workerQueueFilter[filter][partnerIdNotIn]
      - in: query
        name: workerQueueFilter[filter][priorityEqual]
      - in: query
        name: workerQueueFilter[filter][priorityGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][priorityIn]
      - in: query
        name: workerQueueFilter[filter][priorityLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][priorityNotIn]
      - in: query
        name: workerQueueFilter[filter][queueTimeGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][queueTimeLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][statusEqual]
        description: 'Enum Type: `KalturaBatchJobStatus`'
      - in: query
        name: workerQueueFilter[filter][statusIn]
      - in: query
        name: workerQueueFilter[filter][statusNotIn]
      - in: query
        name: workerQueueFilter[filter][updatedAtGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][updatedAtLessThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][urgencyGreaterThanOrEqual]
      - in: query
        name: workerQueueFilter[filter][urgencyLessThanOrEqual]
      - in: query
        name: workerQueueFilter[jobType]
        description: 'Enum Type: `KalturaBatchJobType`'
      - in: query
        name: workerQueueFilter[schedulerId]
      - in: query
        name: workerQueueFilter[workerId]
      responses:
        200:
          description: OK
      tags:
      - Service
      - Batch
      - Action
      - GetQueueSize
---