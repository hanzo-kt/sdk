
# KmsSdkEnvelopeIdentity

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **scheme** | **kotlin.Int** | NodeID scheme. 0x42 &#x3D; ML-DSA-65. |  |
| **node** | **kotlin.String** | 20-byte canonical NodeID (cb58), the SHAKE256-384 digest prefix. |  |
| **digest** | **kotlin.ByteArray** | 48-byte SHAKE256-384 FullDigest commitment (base64). |  |
| **path** | **kotlin.String** | BIP-44 service path the identity was derived from (e.g. hanzo/kms-operator). |  |
| **pubkey** | **kotlin.ByteArray** | ML-DSA-65 public key (base64), for offline verification. |  |



