
# EngineGPUType

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **model** | **kotlin.String** | GPU model name |  [optional] |
| **memoryGb** | **kotlin.Int** |  |  [optional] |
| **architecture** | [**inline**](#Architecture) |  |  [optional] |
| **fp16Tflops** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **bf16Tflops** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **fp8Tflops** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **interconnect** | [**inline**](#Interconnect) |  |  [optional] |
| **totalCount** | **kotlin.Int** |  |  [optional] |
| **availableCount** | **kotlin.Int** |  |  [optional] |


<a id="Architecture"></a>
## Enum: architecture
| Name | Value |
| ---- | ----- |
| architecture | Ampere, Hopper, Ada_Lovelace, Blackwell |


<a id="Interconnect"></a>
## Enum: interconnect
| Name | Value |
| ---- | ----- |
| interconnect | PCIe, NVLink, NVSwitch |



