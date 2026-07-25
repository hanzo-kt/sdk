
# StreamCreateTopicRequestConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **retentionMs** | **kotlin.Int** |  |  [optional] |
| **cleanupPolicy** | [**inline**](#CleanupPolicy) |  |  [optional] |
| **compressionType** | [**inline**](#CompressionType) |  |  [optional] |


<a id="CleanupPolicy"></a>
## Enum: cleanup_policy
| Name | Value |
| ---- | ----- |
| cleanupPolicy | delete, compact |


<a id="CompressionType"></a>
## Enum: compression_type
| Name | Value |
| ---- | ----- |
| compressionType | none, gzip, snappy, lz4, zstd |



