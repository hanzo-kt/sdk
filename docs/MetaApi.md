# MetaApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldHealth**](MetaApi.md#worldWorldHealth) | **GET** /v1/world/health | Liveness probe |
| [**worldWorldVersion**](MetaApi.md#worldWorldVersion) | **GET** /v1/world/version | Build version |


<a id="worldWorldHealth"></a>
# **worldWorldHealth**
> kotlin.Any worldWorldHealth()

Liveness probe

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetaApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetaApi#worldWorldHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetaApi#worldWorldHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="worldWorldVersion"></a>
# **worldWorldVersion**
> kotlin.Any worldWorldVersion()

Build version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MetaApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldVersion()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MetaApi#worldWorldVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MetaApi#worldWorldVersion")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

