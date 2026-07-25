
# PaasDOKSCluster

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **region** | **kotlin.String** |  |  [optional] |
| **version** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **nodeCount** | **kotlin.Int** |  |  [optional] |
| **nodePools** | [**kotlin.collections.List&lt;PaasNodePool&gt;**](PaasNodePool.md) |  |  [optional] |
| **ha** | **kotlin.Boolean** |  |  [optional] |
| **endpoint** | [**java.net.URI**](java.net.URI.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | provisioning, running, degraded, error, deleted |



