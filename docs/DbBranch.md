
# DbBranch

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **projectId** | **kotlin.String** |  |  [optional] |
| **parentId** | **kotlin.String** | Parent branch ID (null for root) |  [optional] |
| **parentLsn** | **kotlin.String** | LSN at which branch was forked |  [optional] |
| **parentTimestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp at which branch was forked |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **currentState** | [**inline**](#CurrentState) |  |  [optional] |
| **logicalSize** | **kotlin.Long** |  |  [optional] |
| **primary** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="CurrentState"></a>
## Enum: current_state
| Name | Value |
| ---- | ----- |
| currentState | init, ready, deleting |



