
# O11yLogLine

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **ts** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | RFC3339 UTC timestamp. |  [optional] |
| **tsNano** | **kotlin.Long** | Nanosecond epoch cursor. Pass the response nextCursor back as sinceNs to tail. |  [optional] |
| **severity** | **kotlin.String** | INFO, WARN, ERROR, etc. |  [optional] |
| **body** | **kotlin.String** |  |  [optional] |
| **source** | [**inline**](#Source) | infra is the raw stdout stream (SuperAdmin only); request is the per-org request log. |  [optional] |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | infra, request |



