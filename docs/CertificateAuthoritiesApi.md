# CertificateAuthoritiesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateCertificateAuthority**](CertificateAuthoritiesApi.md#kmsCreateCertificateAuthority) | **POST** /v1/kms/cert-manager/ca | Create a certificate authority |
| [**kmsDeleteCertificateAuthority**](CertificateAuthoritiesApi.md#kmsDeleteCertificateAuthority) | **DELETE** /v1/kms/cert-manager/ca/{caId} | Delete a certificate authority |
| [**kmsGetCertificateAuthority**](CertificateAuthoritiesApi.md#kmsGetCertificateAuthority) | **GET** /v1/kms/cert-manager/ca/{caId} | Get a certificate authority by ID |
| [**kmsUpdateCertificateAuthority**](CertificateAuthoritiesApi.md#kmsUpdateCertificateAuthority) | **PATCH** /v1/kms/cert-manager/ca/{caId} | Update a certificate authority |


<a id="kmsCreateCertificateAuthority"></a>
# **kmsCreateCertificateAuthority**
> KmsCreateCertificateAuthority200Response kmsCreateCertificateAuthority(kmsCreateCertificateAuthorityRequest)

Create a certificate authority

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificateAuthoritiesApi()
val kmsCreateCertificateAuthorityRequest : KmsCreateCertificateAuthorityRequest =  // KmsCreateCertificateAuthorityRequest | 
try {
    val result : KmsCreateCertificateAuthority200Response = apiInstance.kmsCreateCertificateAuthority(kmsCreateCertificateAuthorityRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificateAuthoritiesApi#kmsCreateCertificateAuthority")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificateAuthoritiesApi#kmsCreateCertificateAuthority")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateCertificateAuthorityRequest** | [**KmsCreateCertificateAuthorityRequest**](KmsCreateCertificateAuthorityRequest.md)|  | |

### Return type

[**KmsCreateCertificateAuthority200Response**](KmsCreateCertificateAuthority200Response.md)

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

<a id="kmsDeleteCertificateAuthority"></a>
# **kmsDeleteCertificateAuthority**
> kotlin.Any kmsDeleteCertificateAuthority(caId)

Delete a certificate authority

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificateAuthoritiesApi()
val caId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteCertificateAuthority(caId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificateAuthoritiesApi#kmsDeleteCertificateAuthority")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificateAuthoritiesApi#kmsDeleteCertificateAuthority")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **caId** | **java.util.UUID**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kmsGetCertificateAuthority"></a>
# **kmsGetCertificateAuthority**
> KmsCreateCertificateAuthority200Response kmsGetCertificateAuthority(caId)

Get a certificate authority by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificateAuthoritiesApi()
val caId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateCertificateAuthority200Response = apiInstance.kmsGetCertificateAuthority(caId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificateAuthoritiesApi#kmsGetCertificateAuthority")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificateAuthoritiesApi#kmsGetCertificateAuthority")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **caId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateCertificateAuthority200Response**](KmsCreateCertificateAuthority200Response.md)

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

<a id="kmsUpdateCertificateAuthority"></a>
# **kmsUpdateCertificateAuthority**
> KmsCreateCertificateAuthority200Response kmsUpdateCertificateAuthority(caId, dnsUpdateZoneRequest)

Update a certificate authority

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CertificateAuthoritiesApi()
val caId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val dnsUpdateZoneRequest : DnsUpdateZoneRequest =  // DnsUpdateZoneRequest | 
try {
    val result : KmsCreateCertificateAuthority200Response = apiInstance.kmsUpdateCertificateAuthority(caId, dnsUpdateZoneRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CertificateAuthoritiesApi#kmsUpdateCertificateAuthority")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CertificateAuthoritiesApi#kmsUpdateCertificateAuthority")
    e.printStackTrace()
}
```

### Parameters
| **caId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dnsUpdateZoneRequest** | [**DnsUpdateZoneRequest**](DnsUpdateZoneRequest.md)|  | |

### Return type

[**KmsCreateCertificateAuthority200Response**](KmsCreateCertificateAuthority200Response.md)

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

