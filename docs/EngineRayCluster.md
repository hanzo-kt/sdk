
# EngineRayCluster

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  [optional] |
| **namespace** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **head** | [**EngineRayClusterHead**](EngineRayClusterHead.md) |  |  [optional] |
| **workers** | [**kotlin.collections.List&lt;EngineRayClusterWorkersInner&gt;**](EngineRayClusterWorkersInner.md) |  |  [optional] |
| **rayVersion** | **kotlin.String** |  |  [optional] |
| **dashboardUrl** | [**java.net.URI**](java.net.URI.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | creating, running, suspended, failed, deleting |



