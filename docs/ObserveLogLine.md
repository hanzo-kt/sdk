
# ObserveLogLine

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **ts** | **kotlin.String** | RFC3339 timestamp (UTC). |  [optional] |
| **tsNano** | **kotlin.Long** | Nanosecond cursor. |  [optional] |
| **severity** | **kotlin.String** | INFO | WARN | ERROR | ... |  [optional] |
| **body** | **kotlin.String** |  |  [optional] |
| **source** | [**inline**](#Source) | \&quot;infra\&quot; (stdout) or \&quot;request\&quot; (org request log). |  [optional] |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | infra, request |



