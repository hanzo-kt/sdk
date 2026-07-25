
# KmsCreateSecretRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **secretKey** | **kotlin.String** |  |  |
| **secretValue** | **kotlin.String** |  |  |
| **secretPath** | **kotlin.String** |  |  |
| **environment** | **kotlin.String** |  |  |
| **secretComment** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **tagIds** | [**kotlin.collections.List&lt;java.util.UUID&gt;**](java.util.UUID.md) |  |  [optional] |
| **secretMetadata** | [**kotlin.collections.List&lt;KmsCreateSecretRequestSecretMetadataInner&gt;**](KmsCreateSecretRequestSecretMetadataInner.md) |  |  [optional] |
| **secretReminderNote** | **kotlin.String** |  |  [optional] |
| **secretReminderRepeatDays** | **kotlin.Int** |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | shared, personal |



