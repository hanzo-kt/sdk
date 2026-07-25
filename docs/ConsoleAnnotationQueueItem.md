
# ConsoleAnnotationQueueItem

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **queueId** | **kotlin.String** |  |  [optional] |
| **objectType** | [**inline**](#ObjectType) |  |  [optional] |
| **objectId** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **completedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **assignedUserId** | **kotlin.String** |  |  [optional] |


<a id="ObjectType"></a>
## Enum: objectType
| Name | Value |
| ---- | ----- |
| objectType | TRACE, OBSERVATION |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | PENDING, COMPLETED, SKIPPED |



