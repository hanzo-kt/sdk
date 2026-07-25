
# MlDeployment

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **modelId** | **kotlin.String** |  |  [optional] |
| **modelVersion** | **kotlin.String** |  |  [optional] |
| **runtime** | [**inline**](#Runtime) |  |  [optional] |
| **gpu** | [**inline**](#Gpu) |  |  [optional] |
| **replicas** | **kotlin.Int** |  |  [optional] |
| **environment** | [**inline**](#Environment) |  |  [optional] |
| **endpoint** | [**java.net.URI**](java.net.URI.md) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Runtime"></a>
## Enum: runtime
| Name | Value |
| ---- | ----- |
| runtime | vllm, triton, onnx, custom |


<a id="Gpu"></a>
## Enum: gpu
| Name | Value |
| ---- | ----- |
| gpu | a100, h100, l40s, t4 |


<a id="Environment"></a>
## Enum: environment
| Name | Value |
| ---- | ----- |
| environment | dev, staging, production |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | deploying, active, failed, stopped |



