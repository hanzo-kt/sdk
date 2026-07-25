
# MqMessage

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **subject** | **kotlin.String** | Subject the message was published to. |  [optional] |
| **&#x60;data&#x60;** | **kotlin.String** | Message payload (base64-encoded for binary data). |  [optional] |
| **headers** | **kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt;** | Message headers (key to list of values). |  [optional] |
| **reply** | **kotlin.String** | Reply-to subject for request/reply patterns. |  [optional] |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Server timestamp when the message was received. |  [optional] |
| **sequence** | **kotlin.Int** | Stream sequence number (present only for JetStream messages).  |  [optional] |



