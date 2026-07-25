
# KvClusterNodesInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **role** | [**inline**](#Role) |  |  [optional] |
| **host** | **kotlin.String** |  |  [optional] |
| **port** | **kotlin.Int** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **memoryUsedMb** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **memoryMaxMb** | **kotlin.Int** |  |  [optional] |


<a id="Role"></a>
## Enum: role
| Name | Value |
| ---- | ----- |
| role | primary, replica |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | online, offline, syncing |



