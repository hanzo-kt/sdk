
# O11yStatusResult

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **product** | **kotlin.String** |  |  [optional] |
| **up** | **kotlin.Boolean** |  |  [optional] |
| **latencyMs** | **kotlin.Long** |  |  [optional] |
| **source** | [**inline**](#Source) |  |  [optional] |
| **deployments** | [**kotlin.collections.List&lt;O11yDeployment&gt;**](O11yDeployment.md) |  |  [optional] |
| **checkedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | probe, victoria-metrics, unreachable, unknown-service |



