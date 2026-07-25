
# AgentsEventView

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **sessionId** | **kotlin.String** |  |  [optional] |
| **seq** | **kotlin.Long** |  |  [optional] |
| **kind** | [**inline**](#Kind) |  |  [optional] |
| **actor** | **kotlin.String** |  |  [optional] |
| **payload** | [**kotlin.Any**](.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Kind"></a>
## Enum: kind
| Name | Value |
| ---- | ----- |
| kind | message, tool-call, spawn, log, status, control |



