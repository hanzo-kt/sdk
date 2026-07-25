
# MqConsumerConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **durableName** | **kotlin.String** | Durable consumer name. If set, the consumer survives client disconnections.  |  [optional] |
| **filterSubject** | **kotlin.String** | Subject filter. Only messages matching this subject are delivered. Supports wildcards.  |  [optional] |
| **ackPolicy** | [**inline**](#AckPolicy) | Acknowledgment policy. &#x60;explicit&#x60; requires per-message ack. &#x60;all&#x60; acks all messages up to the acked sequence. &#x60;none&#x60; disables acks.  |  [optional] |
| **deliverPolicy** | [**inline**](#DeliverPolicy) | Where to start delivery. &#x60;all&#x60; delivers from the beginning. &#x60;last&#x60; delivers the last message. &#x60;new&#x60; delivers only new messages. &#x60;by_start_sequence&#x60; and &#x60;by_start_time&#x60; start from a specific point.  |  [optional] |
| **optStartSeq** | **kotlin.Int** | Starting sequence number (used with deliver_policy &#x60;by_start_sequence&#x60;).  |  [optional] |
| **optStartTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Starting timestamp (used with deliver_policy &#x60;by_start_time&#x60;).  |  [optional] |
| **maxDeliver** | **kotlin.Int** | Maximum delivery attempts before the message is dropped or sent to a dead letter subject (-1 for unlimited).  |  [optional] |
| **ackWait** | **kotlin.String** | Time to wait for acknowledgment before redelivery (e.g., \&quot;30s\&quot;, \&quot;5m\&quot;). Defaults to \&quot;30s\&quot;.  |  [optional] |
| **replayPolicy** | [**inline**](#ReplayPolicy) | Replay policy for historical messages. &#x60;instant&#x60; delivers as fast as possible. &#x60;original&#x60; preserves original timing gaps.  |  [optional] |
| **maxAckPending** | **kotlin.Int** | Maximum number of unacknowledged messages before delivery pauses.  |  [optional] |
| **description** | **kotlin.String** | Optional human-readable description. |  [optional] |


<a id="AckPolicy"></a>
## Enum: ack_policy
| Name | Value |
| ---- | ----- |
| ackPolicy | none, all, explicit |


<a id="DeliverPolicy"></a>
## Enum: deliver_policy
| Name | Value |
| ---- | ----- |
| deliverPolicy | all, last, new, by_start_sequence, by_start_time, last_per_subject |


<a id="ReplayPolicy"></a>
## Enum: replay_policy
| Name | Value |
| ---- | ----- |
| replayPolicy | instant, original |



