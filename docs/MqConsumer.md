
# MqConsumer

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  [optional] |
| **streamName** | **kotlin.String** |  |  [optional] |
| **config** | [**MqConsumerConfig**](MqConsumerConfig.md) |  |  [optional] |
| **delivered** | [**MqSequencePair**](MqSequencePair.md) |  |  [optional] |
| **ackFloor** | [**MqSequencePair**](MqSequencePair.md) |  |  [optional] |
| **numPending** | **kotlin.Int** | Messages waiting to be delivered. |  [optional] |
| **numRedelivered** | **kotlin.Int** | Messages currently being redelivered. |  [optional] |
| **numWaiting** | **kotlin.Int** | Pull requests waiting for messages. |  [optional] |
| **numAckPending** | **kotlin.Int** | Messages delivered but not yet acknowledged. |  [optional] |
| **created** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



