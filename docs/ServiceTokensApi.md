# ServiceTokensApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsGetServiceToken**](ServiceTokensApi.md#kmsGetServiceToken) | **GET** /v1/kms/service-token | Get the service token associated with the current request |


<a id="kmsGetServiceToken"></a>
# **kmsGetServiceToken**
> KmsGetServiceToken200Response kmsGetServiceToken()

Get the service token associated with the current request

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServiceTokensApi()
try {
    val result : KmsGetServiceToken200Response = apiInstance.kmsGetServiceToken()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceTokensApi#kmsGetServiceToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceTokensApi#kmsGetServiceToken")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsGetServiceToken200Response**](KmsGetServiceToken200Response.md)

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

