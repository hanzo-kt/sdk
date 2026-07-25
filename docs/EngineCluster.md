
# EngineCluster

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **provider** | [**inline**](#Provider) |  |  [optional] |
| **region** | **kotlin.String** |  |  [optional] |
| **nodeCount** | **kotlin.Int** |  |  [optional] |
| **totalGpus** | **kotlin.Int** |  |  [optional] |
| **availableGpus** | **kotlin.Int** |  |  [optional] |
| **gpuTypes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **totalMemoryGb** | **kotlin.Int** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | online, offline, degraded, provisioning |


<a id="Provider"></a>
## Enum: provider
| Name | Value |
| ---- | ----- |
| provider | bare_metal, aws, gcp, azure, lambda, coreweave |



