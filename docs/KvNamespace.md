
# KvNamespace

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **maxMemoryMb** | **kotlin.Int** | Memory limit in MB |  [optional] |
| **usedMemoryMb** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **keyCount** | **kotlin.Int** |  |  [optional] |
| **evictionPolicy** | [**inline**](#EvictionPolicy) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="EvictionPolicy"></a>
## Enum: eviction_policy
| Name | Value |
| ---- | ----- |
| evictionPolicy | noeviction, allkeys-lru, allkeys-lfu, volatile-lru, volatile-lfu, allkeys-random, volatile-random, volatile-ttl |



