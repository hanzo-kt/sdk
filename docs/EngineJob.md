
# EngineJob

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **clusterId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **image** | **kotlin.String** | Container image |  [optional] |
| **command** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **resources** | [**EngineJobResources**](EngineJobResources.md) |  |  [optional] |
| **env** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |
| **priority** | **kotlin.Int** |  |  [optional] |
| **maxRetries** | **kotlin.Int** |  |  [optional] |
| **timeoutSeconds** | **kotlin.Int** |  |  [optional] |
| **metrics** | [**EngineJobMetrics**](EngineJobMetrics.md) |  |  [optional] |
| **startedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **completedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | training, inference, fine_tune, evaluation |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, scheduling, running, succeeded, failed, cancelled |



