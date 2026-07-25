
# MqKVBucketConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Bucket name. |  |
| **history** | **kotlin.Int** | Maximum number of revisions per key. |  [optional] |
| **ttl** | **kotlin.String** | Default TTL for keys (e.g., \&quot;1h\&quot;, \&quot;7d\&quot;, \&quot;0\&quot; for no expiry).  |  [optional] |
| **maxValueSize** | **kotlin.Int** | Maximum value size in bytes (-1 for default). |  [optional] |
| **maxBytes** | **kotlin.Long** | Maximum total bucket size (-1 for unlimited). |  [optional] |
| **storage** | [**inline**](#Storage) | Storage backend. |  [optional] |
| **numReplicas** | **kotlin.Int** | Number of replicas. |  [optional] |
| **description** | **kotlin.String** | Optional human-readable description. |  [optional] |


<a id="Storage"></a>
## Enum: storage
| Name | Value |
| ---- | ----- |
| storage | file, memory |



