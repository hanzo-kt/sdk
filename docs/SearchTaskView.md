
# SearchTaskView

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **uid** | **kotlin.Int** |  |  [optional] |
| **indexUid** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **type** | **kotlin.String** |  |  [optional] |
| **canceledBy** | **kotlin.Int** |  |  [optional] |
| **details** | [**kotlin.Any**](.md) |  |  [optional] |
| **error** | [**SearchResponseError**](SearchResponseError.md) |  |  [optional] |
| **duration** | **kotlin.String** |  |  [optional] |
| **enqueuedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **startedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **finishedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | enqueued, processing, succeeded, failed, canceled |



