
# KmsCertificateAuthority

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **friendlyName** | **kotlin.String** |  |  [optional] |
| **organization** | **kotlin.String** |  |  [optional] |
| **commonName** | **kotlin.String** |  |  [optional] |
| **dn** | **kotlin.String** |  |  [optional] |
| **maxPathLength** | **kotlin.Int** |  |  [optional] |
| **keyAlgorithm** | [**inline**](#KeyAlgorithm) |  |  [optional] |
| **notBefore** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **notAfter** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | root, intermediate |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, disabled, pending-certificate |


<a id="KeyAlgorithm"></a>
## Enum: keyAlgorithm
| Name | Value |
| ---- | ----- |
| keyAlgorithm | RSA_2048, RSA_4096, ECDSA_P256, ECDSA_P384 |



