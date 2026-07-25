# CertificatesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsGetCertificate**](CertificatesApi.md#kmsGetCertificate) | **GET** /v1/kms/cert-manager/certificates/{certificateId} | Get a certificate by ID |
| [**kmsIssueCertificate**](CertificatesApi.md#kmsIssueCertificate) | **POST** /v1/kms/cert-manager/ca/{caId}/issue-certificate | Issue a certificate from a CA |
| [**kmsListCertificates**](CertificatesApi.md#kmsListCertificates) | **GET** /v1/kms/cert-manager/certificates | List certificates |
| [**kmsRevokeCertificate**](CertificatesApi.md#kmsRevokeCertificate) | **DELETE** /v1/kms/cert-manager/certificates/{certificateId} | Revoke a certificate |


<a id="kmsGetCertificate"></a>
# **kmsGetCertificate**
> KmsGetCertificate200Response kmsGetCertificate(certificateId)

Get a certificate by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificatesApi()
val certificateId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsGetCertificate200Response = apiInstance.kmsGetCertificate(certificateId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificatesApi#kmsGetCertificate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificatesApi#kmsGetCertificate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **certificateId** | **java.util.UUID**|  | |

### Return type

[**KmsGetCertificate200Response**](KmsGetCertificate200Response.md)

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

<a id="kmsIssueCertificate"></a>
# **kmsIssueCertificate**
> KmsIssueCertificate200Response kmsIssueCertificate(caId, kmsIssueCertificateRequest)

Issue a certificate from a CA

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificatesApi()
val caId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsIssueCertificateRequest : KmsIssueCertificateRequest =  // KmsIssueCertificateRequest | 
try {
    val result : KmsIssueCertificate200Response = apiInstance.kmsIssueCertificate(caId, kmsIssueCertificateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificatesApi#kmsIssueCertificate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificatesApi#kmsIssueCertificate")
    e.printStackTrace()
}
```

### Parameters
| **caId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsIssueCertificateRequest** | [**KmsIssueCertificateRequest**](KmsIssueCertificateRequest.md)|  | |

### Return type

[**KmsIssueCertificate200Response**](KmsIssueCertificate200Response.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="kmsListCertificates"></a>
# **kmsListCertificates**
> KmsListCertificates200Response kmsListCertificates(caId, offset, limit)

List certificates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificatesApi()
val caId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KmsListCertificates200Response = apiInstance.kmsListCertificates(caId, offset, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificatesApi#kmsListCertificates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificatesApi#kmsListCertificates")
    e.printStackTrace()
}
```

### Parameters
| **caId** | **java.util.UUID**|  | [optional] |
| **offset** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**KmsListCertificates200Response**](KmsListCertificates200Response.md)

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

<a id="kmsRevokeCertificate"></a>
# **kmsRevokeCertificate**
> kotlin.Any kmsRevokeCertificate(certificateId, kmsRevokeCertificateRequest)

Revoke a certificate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificatesApi()
val certificateId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsRevokeCertificateRequest : KmsRevokeCertificateRequest =  // KmsRevokeCertificateRequest | 
try {
    val result : kotlin.Any = apiInstance.kmsRevokeCertificate(certificateId, kmsRevokeCertificateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificatesApi#kmsRevokeCertificate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificatesApi#kmsRevokeCertificate")
    e.printStackTrace()
}
```

### Parameters
| **certificateId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsRevokeCertificateRequest** | [**KmsRevokeCertificateRequest**](KmsRevokeCertificateRequest.md)|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

