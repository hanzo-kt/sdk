
# EngineClusterNode

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **gpus** | [**kotlin.collections.List&lt;EngineGPUDevice&gt;**](EngineGPUDevice.md) |  |  [optional] |
| **cpuCores** | **kotlin.Int** |  |  [optional] |
| **memoryGb** | **kotlin.Int** |  |  [optional] |
| **ip** | **kotlin.String** |  |  [optional] |
| **labels** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ready, not_ready, cordoned, draining |



