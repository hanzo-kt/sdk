
# EngineJobCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **type** | [**inline**](#Type) |  |  |
| **image** | **kotlin.String** |  |  |
| **resources** | [**EngineJobResources**](EngineJobResources.md) |  |  |
| **clusterId** | [**java.util.UUID**](java.util.UUID.md) | Target cluster (auto-selected if omitted) |  [optional] |
| **command** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **env** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |
| **priority** | **kotlin.Int** |  |  [optional] |
| **maxRetries** | **kotlin.Int** |  |  [optional] |
| **timeoutSeconds** | **kotlin.Int** |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | training, inference, fine_tune, evaluation |



