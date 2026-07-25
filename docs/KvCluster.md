
# KvCluster

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **version** | **kotlin.String** | Server version |  [optional] |
| **mode** | [**inline**](#Mode) |  |  [optional] |
| **nodes** | [**kotlin.collections.List&lt;KvClusterNodesInner&gt;**](KvClusterNodesInner.md) |  |  [optional] |
| **replicas** | **kotlin.Int** |  |  [optional] |
| **maxMemoryMb** | **kotlin.Int** |  |  [optional] |
| **connectionUri** | **kotlin.String** | Connection string (valkey://...) |  [optional] |
| **tls** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | provisioning, running, degraded, stopped, deleted |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | standalone, sentinel, cluster |



