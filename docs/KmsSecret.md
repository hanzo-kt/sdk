
# KmsSecret

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **version** | **kotlin.Int** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **secretKey** | **kotlin.String** |  |  [optional] |
| **secretValue** | **kotlin.String** |  |  [optional] |
| **secretComment** | **kotlin.String** |  |  [optional] |
| **secretPath** | **kotlin.String** |  |  [optional] |
| **environment** | **kotlin.String** |  |  [optional] |
| **tags** | [**kotlin.collections.List&lt;KmsSecretTag&gt;**](KmsSecretTag.md) |  |  [optional] |
| **secretMetadata** | [**kotlin.collections.List&lt;KmsCreateSecretRequestSecretMetadataInner&gt;**](KmsCreateSecretRequestSecretMetadataInner.md) |  |  [optional] |
| **secretReminderNote** | **kotlin.String** |  |  [optional] |
| **secretReminderRepeatDays** | **kotlin.Int** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | shared, personal |



