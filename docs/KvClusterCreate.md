
# KvClusterCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **mode** | [**inline**](#Mode) |  |  [optional] |
| **version** | **kotlin.String** |  |  [optional] |
| **maxMemoryMb** | **kotlin.Int** |  |  [optional] |
| **replicas** | **kotlin.Int** |  |  [optional] |
| **tls** | **kotlin.Boolean** |  |  [optional] |
| **evictionPolicy** | [**inline**](#EvictionPolicy) |  |  [optional] |


<a id="Mode"></a>
## Enum: mode
| Name | Value |
| ---- | ----- |
| mode | standalone, sentinel, cluster |


<a id="EvictionPolicy"></a>
## Enum: eviction_policy
| Name | Value |
| ---- | ----- |
| evictionPolicy | noeviction, allkeys-lru, allkeys-lfu, volatile-lru, volatile-lfu, allkeys-random |



