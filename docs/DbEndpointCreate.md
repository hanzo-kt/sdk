
# DbEndpointCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String** |  |  |
| **type** | [**inline**](#Type) |  |  |
| **settings** | [**DbEndpointSettings**](DbEndpointSettings.md) |  |  [optional] |
| **poolerEnabled** | **kotlin.Boolean** |  |  [optional] |
| **poolerMode** | [**inline**](#PoolerMode) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | read_write, read_only |


<a id="PoolerMode"></a>
## Enum: pooler_mode
| Name | Value |
| ---- | ----- |
| poolerMode | transaction, session |



