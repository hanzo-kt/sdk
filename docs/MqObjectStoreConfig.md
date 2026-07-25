
# MqObjectStoreConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Store name. |  |
| **maxChunkSize** | **kotlin.Int** | Maximum chunk size in bytes (default 128KB). |  [optional] |
| **maxBytes** | **kotlin.Long** | Maximum total store size (-1 for unlimited). |  [optional] |
| **storage** | [**inline**](#Storage) | Storage backend. |  [optional] |
| **numReplicas** | **kotlin.Int** | Number of replicas. |  [optional] |
| **description** | **kotlin.String** | Optional human-readable description. |  [optional] |


<a id="Storage"></a>
## Enum: storage
| Name | Value |
| ---- | ----- |
| storage | file, memory |



