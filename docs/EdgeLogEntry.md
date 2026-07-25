
# EdgeLogEntry

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **eventType** | [**inline**](#EventType) |  |  [optional] |
| **level** | [**inline**](#Level) |  |  [optional] |
| **message** | **kotlin.String** |  |  [optional] |
| **executionId** | **kotlin.String** |  |  [optional] |


<a id="EventType"></a>
## Enum: event_type
| Name | Value |
| ---- | ----- |
| eventType | uncaughtException, log, boot, beforeUnload |


<a id="Level"></a>
## Enum: level
| Name | Value |
| ---- | ----- |
| level | info, warn, error, debug |



