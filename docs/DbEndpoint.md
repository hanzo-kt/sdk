
# DbEndpoint

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **host** | **kotlin.String** |  |  [optional] |
| **projectId** | **kotlin.String** |  |  [optional] |
| **branchId** | **kotlin.String** |  |  [optional] |
| **regionId** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **currentState** | [**inline**](#CurrentState) |  |  [optional] |
| **settings** | [**DbEndpointSettings**](DbEndpointSettings.md) |  |  [optional] |
| **poolerEnabled** | **kotlin.Boolean** |  |  [optional] |
| **poolerMode** | [**inline**](#PoolerMode) |  |  [optional] |
| **lastActive** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | read_write, read_only |


<a id="CurrentState"></a>
## Enum: current_state
| Name | Value |
| ---- | ----- |
| currentState | init, active, idle, suspended |


<a id="PoolerMode"></a>
## Enum: pooler_mode
| Name | Value |
| ---- | ----- |
| poolerMode | transaction, session |



