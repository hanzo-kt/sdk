
# EngineGPUDevice

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **index** | **kotlin.Int** |  |  [optional] |
| **model** | **kotlin.String** | GPU model (e.g. A100-SXM4-80GB, H100-SXM5-80GB) |  [optional] |
| **memoryMb** | **kotlin.Int** |  |  [optional] |
| **utilizationPercent** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **memoryUsedMb** | **kotlin.Int** |  |  [optional] |
| **temperatureC** | **kotlin.Int** |  |  [optional] |
| **powerDrawW** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | idle, allocated, error |



