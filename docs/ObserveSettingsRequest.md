
# ObserveSettingsRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **config** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) | Non-secret config; stored verbatim (bounded at 64KiB). |  [optional] |
| **secrets** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** | Secret fields; VALUES routed to KMS, never SQLite. Each key must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;; each value is bounded at 8KiB. An empty value or the mask sentinel (&#x60;••••••••&#x60;) means \&quot;unchanged\&quot;. Max 64 fields.  |  [optional] |



