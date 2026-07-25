
# PubsubStreamConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Unique stream name |  |
| **subjects** | **kotlin.collections.List&lt;kotlin.String&gt;** | Subjects captured by this stream |  |
| **storage** | [**inline**](#Storage) | Storage backend |  [optional] |
| **replicas** | [**inline**](#Replicas) | Replication factor |  [optional] |
| **retention** | [**inline**](#Retention) |  |  [optional] |
| **maxMsgs** | **kotlin.Int** | Maximum messages to retain |  [optional] |
| **maxBytes** | **kotlin.Int** | Maximum bytes to retain |  [optional] |
| **maxAge** | **kotlin.Int** | Maximum age in nanoseconds (0 &#x3D; unlimited) |  [optional] |
| **discard** | [**inline**](#Discard) | Discard policy when limits are reached |  [optional] |


<a id="Storage"></a>
## Enum: storage
| Name | Value |
| ---- | ----- |
| storage | file, memory |


<a id="Replicas"></a>
## Enum: replicas
| Name | Value |
| ---- | ----- |
| replicas | 1, 3, 5 |


<a id="Retention"></a>
## Enum: retention
| Name | Value |
| ---- | ----- |
| retention | limits, interest, workqueue |


<a id="Discard"></a>
## Enum: discard
| Name | Value |
| ---- | ----- |
| discard | old, new |



