
# KmsCertificate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **caId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **friendlyName** | **kotlin.String** |  |  [optional] |
| **commonName** | **kotlin.String** |  |  [optional] |
| **serialNumber** | **kotlin.String** |  |  [optional] |
| **notBefore** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **notAfter** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, revoked |



