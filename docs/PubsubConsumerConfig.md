
# PubsubConsumerConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **durableName** | **kotlin.String** | Durable consumer name |  |
| **deliverPolicy** | [**inline**](#DeliverPolicy) |  |  [optional] |
| **ackPolicy** | [**inline**](#AckPolicy) |  |  [optional] |
| **filterSubject** | **kotlin.String** | Subject filter for this consumer |  [optional] |
| **maxDeliver** | **kotlin.Int** | Maximum delivery attempts per message |  [optional] |
| **ackWait** | **kotlin.Long** | Ack wait timeout in nanoseconds |  [optional] |


<a id="DeliverPolicy"></a>
## Enum: deliver_policy
| Name | Value |
| ---- | ----- |
| deliverPolicy | all, last, new, by_start_sequence, by_start_time, last_per_subject |


<a id="AckPolicy"></a>
## Enum: ack_policy
| Name | Value |
| ---- | ----- |
| ackPolicy | explicit, none, all |



