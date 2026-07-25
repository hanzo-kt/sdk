# SDKApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsSdkSecretsOp**](SDKApi.md#kmsSdkSecretsOp) | **POST** /v1/sdk/secrets | Enveloped secret + threshold-key operation |


<a id="kmsSdkSecretsOp"></a>
# **kmsSdkSecretsOp**
> kotlin.Any kmsSdkSecretsOp(kmsSdkEnvelope)

Enveloped secret + threshold-key operation

The SDK-facing native secrets plane. A single RPC endpoint: the body is a signed Envelope (ML-DSA-65 over the request), and the OPERATION is the signed &#x60;op&#x60; field — never the URL. Authorization is consensus-native: the caller&#39;s mnemonic-derived NodeID must be in the validator authority (reads: OpSecretGet 0x0040, OpSecretList 0x0042, OpVerify 0x0051) and, for writes (OpSecretPut 0x0041 — also the rotate op, OpSecretDelete 0x0043, OpSign 0x0050), additionally in the operator authority. Every envelope is verified for signature, wall-clock freshness (±5m), and replay (per-(NodeID,nonce) ledger) before dispatch. There is NO bearer token on this surface — the ML-DSA-65 envelope IS the credential. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SDKApi()
val kmsSdkEnvelope : KmsSdkEnvelope =  // KmsSdkEnvelope | 
try {
    val result : kotlin.Any = apiInstance.kmsSdkSecretsOp(kmsSdkEnvelope)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SDKApi#kmsSdkSecretsOp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SDKApi#kmsSdkSecretsOp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsSdkEnvelope** | [**KmsSdkEnvelope**](KmsSdkEnvelope.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

