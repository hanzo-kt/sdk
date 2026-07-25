
# EngineServingEndpoint

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  [optional] |
| **model** | **kotlin.String** | Model identifier or path |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **replicas** | **kotlin.Int** |  |  [optional] |
| **minReplicas** | **kotlin.Int** |  |  [optional] |
| **maxReplicas** | **kotlin.Int** |  |  [optional] |
| **gpuType** | **kotlin.String** |  |  [optional] |
| **gpuPerReplica** | **kotlin.Int** |  |  [optional] |
| **framework** | [**inline**](#Framework) |  |  [optional] |
| **url** | [**java.net.URI**](java.net.URI.md) | Inference endpoint URL |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | provisioning, running, scaling, failed, stopped |


<a id="Framework"></a>
## Enum: framework
| Name | Value |
| ---- | ----- |
| framework | vllm, tgi, triton, custom |



