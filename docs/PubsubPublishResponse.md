
# PubsubPublishResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **ok** | **kotlin.Boolean** |  |  [optional] |
| **stream** | **kotlin.String** | JetStream stream name (if subject is captured) |  [optional] |
| **seq** | **kotlin.Int** | JetStream sequence number |  [optional] |
| **duplicate** | **kotlin.Boolean** | Whether message was a duplicate (dedup by Msg-Id header) |  [optional] |



