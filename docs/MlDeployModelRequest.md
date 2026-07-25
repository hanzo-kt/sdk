
# MlDeployModelRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **modelId** | **kotlin.String** |  |  |
| **modelVersion** | **kotlin.String** |  |  [optional] |
| **runtime** | [**inline**](#Runtime) |  |  [optional] |
| **gpu** | [**inline**](#Gpu) |  |  [optional] |
| **replicas** | **kotlin.Int** |  |  [optional] |
| **environment** | [**inline**](#Environment) |  |  [optional] |


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



