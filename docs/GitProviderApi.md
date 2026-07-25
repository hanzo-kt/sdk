# GitProviderApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformGitProviderGetAll**](GitProviderApi.md#platformGitProviderGetAll) | **GET** /v1/platform/gitProvider/getAll | List all git providers |


<a id="platformGitProviderGetAll"></a>
# **platformGitProviderGetAll**
> PlatformTRPCResult platformGitProviderGetAll()

List all git providers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitProviderApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformGitProviderGetAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitProviderApi#platformGitProviderGetAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitProviderApi#platformGitProviderGetAll")
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

