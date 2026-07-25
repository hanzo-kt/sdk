
# DbEndpointSettings

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **autoscalingLimitMinCu** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Minimum compute units (0.25 CU &#x3D; 0.25 vCPU, 1 GB RAM) |  [optional] |
| **autoscalingLimitMaxCu** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Maximum compute units |  [optional] |
| **suspendTimeoutSeconds** | **kotlin.Int** | Seconds of inactivity before suspending (0 &#x3D; never) |  [optional] |
| **pgSettings** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** | PostgreSQL configuration overrides |  [optional] |



