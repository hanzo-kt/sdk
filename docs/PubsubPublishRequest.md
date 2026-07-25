
# PubsubPublishRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **subject** | **kotlin.String** | Subject to publish to (e.g. orders.created) |  |
| **&#x60;data&#x60;** | **kotlin.String** | Message payload (string or base64-encoded binary) |  |
| **headers** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** | Optional message headers |  [optional] |
| **reply** | **kotlin.String** | Reply-to subject for request/reply pattern |  [optional] |



