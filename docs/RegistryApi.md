# RegistryApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformRegistryAll**](RegistryApi.md#platformRegistryAll) | **GET** /v1/platform/registry/all | List container registries |


<a id="platformRegistryAll"></a>
# **platformRegistryAll**
> PlatformTRPCResult platformRegistryAll()

List container registries

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RegistryApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformRegistryAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RegistryApi#platformRegistryAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RegistryApi#platformRegistryAll")
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

