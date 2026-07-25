
# PubsubKVBucketConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String** | Bucket name |  |
| **history** | **kotlin.Int** | Number of historical values per key |  [optional] |
| **ttl** | **kotlin.Int** | Default TTL in nanoseconds (0 &#x3D; no expiry) |  [optional] |
| **replicas** | [**inline**](#Replicas) |  |  [optional] |
| **maxValueSize** | **kotlin.Int** | Maximum value size in bytes |  [optional] |


<a id="Replicas"></a>
## Enum: replicas
| Name | Value |
| ---- | ----- |
| replicas | 1, 3, 5 |



