# CertificateApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformCertificatesAll**](CertificateApi.md#platformCertificatesAll) | **GET** /v1/platform/certificates/all | List SSL certificates (admin) |


<a id="platformCertificatesAll"></a>
# **platformCertificatesAll**
> PlatformTRPCResult platformCertificatesAll()

List SSL certificates (admin)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificateApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformCertificatesAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificateApi#platformCertificatesAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificateApi#platformCertificatesAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

