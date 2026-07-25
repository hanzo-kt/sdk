
# NotifyNotifySend200Response

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **messageId** | **kotlin.String** | Generated 16-byte hex message id (opaque handle). |  |
| **status** | [**inline**](#Status) | Terminal delivery status. In the sync fold this is &#x60;sent&#x60; on success or &#x60;failed&#x60; on terminal failure. (The type also defines &#x60;queued&#x60;, &#x60;sending&#x60;, &#x60;delivered&#x60; for the async plane, which is not folded.)  |  |
| **items** | [**kotlin.collections.List&lt;NotifySendResponse&gt;**](NotifySendResponse.md) |  |  |
| **taskId** | **kotlin.String** | hanzoai/tasks workflow id in async mode; always empty in the sync fold.  |  [optional] |
| **error** | **kotlin.String** | Set on terminal failure (sync mode only). |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | queued, sending, sent, delivered, failed |



