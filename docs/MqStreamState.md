
# MqStreamState

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **messages** | **kotlin.Int** | Total number of messages in the stream. |  [optional] |
| **bytes** | **kotlin.Int** | Total bytes used by the stream. |  [optional] |
| **firstSeq** | **kotlin.Int** | Sequence number of the first message. |  [optional] |
| **firstTs** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp of the first message. |  [optional] |
| **lastSeq** | **kotlin.Int** | Sequence number of the last message. |  [optional] |
| **lastTs** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp of the last message. |  [optional] |
| **consumerCount** | **kotlin.Int** | Number of consumers attached to this stream. |  [optional] |
| **numSubjects** | **kotlin.Int** | Number of unique subjects in the stream. |  [optional] |
| **numDeleted** | **kotlin.Int** | Number of deleted messages (gaps in sequence). |  [optional] |



