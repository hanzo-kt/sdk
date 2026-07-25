# DestinationApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformDestinationAll**](DestinationApi.md#platformDestinationAll) | **GET** /v1/platform/destination/all | List backup destinations |


<a id="platformDestinationAll"></a>
# **platformDestinationAll**
> PlatformTRPCResult platformDestinationAll()

List backup destinations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DestinationApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformDestinationAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DestinationApi#platformDestinationAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DestinationApi#platformDestinationAll")
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

