
# DnsDNSSECStatus

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **enabled** | **kotlin.Boolean** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **algorithm** | **kotlin.String** |  |  [optional] |
| **dsRecord** | **kotlin.String** | DS record to add at registrar |  [optional] |
| **keyTag** | **kotlin.Int** |  |  [optional] |
| **digestType** | **kotlin.String** |  |  [optional] |
| **digest** | **kotlin.String** |  |  [optional] |
| **publicKey** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, pending, disabled |



