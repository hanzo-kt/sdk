
# KmsProject

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **slug** | **kotlin.String** |  |  [optional] |
| **orgId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **environments** | [**kotlin.collections.List&lt;KmsEnvironment&gt;**](KmsEnvironment.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | SecretManager, CertManager |



