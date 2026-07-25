
# MqStreamConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Stream name (alphanumeric, hyphens, underscores). |  |
| **subjects** | **kotlin.collections.List&lt;kotlin.String&gt;** | Subjects bound to this stream. Supports wildcards.  |  |
| **retention** | [**inline**](#Retention) | Message retention policy. &#x60;limits&#x60; keeps messages until limits are hit. &#x60;interest&#x60; keeps messages while consumers exist. &#x60;workqueue&#x60; deletes messages after acknowledgment.  |  [optional] |
| **maxMsgs** | **kotlin.Long** | Maximum number of messages (-1 for unlimited). |  [optional] |
| **maxBytes** | **kotlin.Long** | Maximum total bytes (-1 for unlimited). |  [optional] |
| **maxAge** | **kotlin.String** | Maximum message age (e.g., \&quot;24h\&quot;, \&quot;7d\&quot;, \&quot;0\&quot; for unlimited).  |  [optional] |
| **maxMsgSize** | **kotlin.Int** | Maximum single message size in bytes (-1 for default). |  [optional] |
| **storage** | [**inline**](#Storage) | Storage backend for stream data. |  [optional] |
| **numReplicas** | **kotlin.Int** | Number of replicas in the cluster. |  [optional] |
| **discard** | [**inline**](#Discard) | Discard policy when limits are reached. &#x60;old&#x60; discards the oldest messages. &#x60;new&#x60; rejects new messages.  |  [optional] |
| **duplicateWindow** | **kotlin.String** | Window for message deduplication based on Nats-Msg-Id header (e.g., \&quot;2m\&quot;). Defaults to \&quot;2m\&quot;.  |  [optional] |
| **description** | **kotlin.String** | Optional human-readable description. |  [optional] |


<a id="Retention"></a>
## Enum: retention
| Name | Value |
| ---- | ----- |
| retention | limits, interest, workqueue |


<a id="Storage"></a>
## Enum: storage
| Name | Value |
| ---- | ----- |
| storage | file, memory |


<a id="Discard"></a>
## Enum: discard
| Name | Value |
| ---- | ----- |
| discard | old, new |



