
# GuardSanitizeResultRedactionsInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **type** | [**inline**](#Type) |  |  [optional] |
| **start** | **kotlin.Int** |  |  [optional] |
| **end** | **kotlin.Int** |  |  [optional] |
| **hash** | **kotlin.String** | SHA-256 hash of the original value for audit correlation |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | ssn, credit_card, email, phone, ip, api_key |



