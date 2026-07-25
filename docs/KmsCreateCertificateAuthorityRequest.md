
# KmsCreateCertificateAuthorityRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **projectId** | [**java.util.UUID**](java.util.UUID.md) |  |  |
| **type** | [**inline**](#Type) |  |  |
| **friendlyName** | **kotlin.String** |  |  |
| **commonName** | **kotlin.String** |  |  |
| **keyAlgorithm** | [**inline**](#KeyAlgorithm) |  |  |
| **organization** | **kotlin.String** |  |  [optional] |
| **ou** | **kotlin.String** |  |  [optional] |
| **country** | **kotlin.String** |  |  [optional] |
| **province** | **kotlin.String** |  |  [optional] |
| **locality** | **kotlin.String** |  |  [optional] |
| **maxPathLength** | **kotlin.Int** |  |  [optional] |
| **notAfter** | **kotlin.String** | Duration (e.g., \&quot;10y\&quot;) |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | root, intermediate |


<a id="KeyAlgorithm"></a>
## Enum: keyAlgorithm
| Name | Value |
| ---- | ----- |
| keyAlgorithm | RSA_2048, RSA_4096, ECDSA_P256, ECDSA_P384 |



