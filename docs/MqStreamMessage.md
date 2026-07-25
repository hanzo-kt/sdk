
# MqStreamMessage

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **subject** | **kotlin.String** |  |  [optional] |
| **&#x60;data&#x60;** | **kotlin.String** |  |  [optional] |
| **headers** | **kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt;** |  |  [optional] |
| **sequence** | **kotlin.Int** | Stream sequence number. |  [optional] |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **numDelivered** | **kotlin.Int** | Number of times this message has been delivered. |  [optional] |
| **numPending** | **kotlin.Int** | Messages remaining after this one (consumer context). |  [optional] |



