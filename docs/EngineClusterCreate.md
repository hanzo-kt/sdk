
# EngineClusterCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **provider** | [**inline**](#Provider) |  |  |
| **region** | **kotlin.String** |  |  [optional] |
| **kubeconfig** | **kotlin.String** | Base64-encoded kubeconfig for the cluster |  [optional] |
| **labels** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |


<a id="Provider"></a>
## Enum: provider
| Name | Value |
| ---- | ----- |
| provider | bare_metal, aws, gcp, azure, lambda, coreweave |



