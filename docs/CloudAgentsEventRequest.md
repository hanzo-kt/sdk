
# CloudAgentsEventRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **kind** | [**inline**](#Kind) |  |  |
| **actor** | **kotlin.String** |  |  [optional] |
| **payload** | [**kotlin.Any**](.md) | Opaque JSON blob (validated well-formed, size-bounded). |  [optional] |


<a id="Kind"></a>
## Enum: kind
| Name | Value |
| ---- | ----- |
| kind | message, tool-call, spawn, log, status, control |



