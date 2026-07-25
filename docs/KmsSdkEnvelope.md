
# KmsSdkEnvelope

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **v** | **kotlin.Int** | Envelope version. Only 1 is accepted. |  |
| **id** | [**KmsSdkEnvelopeIdentity**](KmsSdkEnvelopeIdentity.md) |  |  |
| **ts** | **kotlin.Long** | Unix seconds at signing. Rejected outside ±5m of server time. |  |
| **nonce** | **kotlin.String** | Caller-fresh anti-replay nonce (typically 16 random bytes, base64). Reuse within the window is rejected. |  |
| **op** | **kotlin.Int** | Signed operation. 0x0040 get, 0x0041 put (also rotate), 0x0042 list, 0x0043 delete, 0x0050 sign, 0x0051 verify.  |  |
| **req** | [**kotlin.Any**](.md) | Inner request JSON. Shape by op — secrets:{path,name,env[,value]}; sign:{validator_id,key_type,message}; verify adds {signature}.  |  |
| **sig** | **kotlin.ByteArray** | ML-DSA-65 signature (base64) over the canonical digest. |  |



