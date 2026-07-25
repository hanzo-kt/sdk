# SSOApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSsoConfig**](SSOApi.md#kmsCreateSsoConfig) | **POST** /v1/kms/sso/config | Create SSO configuration |
| [**kmsGetSsoConfig**](SSOApi.md#kmsGetSsoConfig) | **GET** /v1/kms/sso/config | Get SSO configuration for an organization |


<a id="kmsCreateSsoConfig"></a>
# **kmsCreateSsoConfig**
> kotlin.Any kmsCreateSsoConfig(kmsCreateSsoConfigRequest)

Create SSO configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SSOApi()
val kmsCreateSsoConfigRequest : KmsCreateSsoConfigRequest =  // KmsCreateSsoConfigRequest | 
try {
    val result : kotlin.Any = apiInstance.kmsCreateSsoConfig(kmsCreateSsoConfigRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SSOApi#kmsCreateSsoConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SSOApi#kmsCreateSsoConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSsoConfigRequest** | [**KmsCreateSsoConfigRequest**](KmsCreateSsoConfigRequest.md)|  | |

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

<a id="kmsGetSsoConfig"></a>
# **kmsGetSsoConfig**
> KmsGetSsoConfig200Response kmsGetSsoConfig(orgId)

Get SSO configuration for an organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SSOApi()
val orgId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsGetSsoConfig200Response = apiInstance.kmsGetSsoConfig(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SSOApi#kmsGetSsoConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SSOApi#kmsGetSsoConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **java.util.UUID**|  | |

### Return type

[**KmsGetSsoConfig200Response**](KmsGetSsoConfig200Response.md)

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

