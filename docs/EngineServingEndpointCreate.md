
# EngineServingEndpointCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **model** | **kotlin.String** |  |  |
| **framework** | [**inline**](#Framework) |  |  [optional] |
| **gpuType** | **kotlin.String** |  |  [optional] |
| **gpuPerReplica** | **kotlin.Int** |  |  [optional] |
| **minReplicas** | **kotlin.Int** |  |  [optional] |
| **maxReplicas** | **kotlin.Int** |  |  [optional] |
| **env** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |
| **scaleToZero** | **kotlin.Boolean** |  |  [optional] |
| **maxBatchSize** | **kotlin.Int** |  |  [optional] |
| **maxConcurrentRequests** | **kotlin.Int** |  |  [optional] |


<a id="Framework"></a>
## Enum: framework
| Name | Value |
| ---- | ----- |
| framework | vllm, tgi, triton, custom |



