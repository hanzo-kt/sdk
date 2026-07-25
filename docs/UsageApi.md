# UsageApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gitGetGitUsage**](UsageApi.md#gitGetGitUsage) | **GET** /v1/git/usage | Per-repo + total storage bytes for the tenant |


<a id="gitGetGitUsage"></a>
# **gitGetGitUsage**
> GitUsage gitGetGitUsage()

Per-repo + total storage bytes for the tenant

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UsageApi()
try {
    val result : GitUsage = apiInstance.gitGetGitUsage()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UsageApi#gitGetGitUsage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UsageApi#gitGetGitUsage")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GitUsage**](GitUsage.md)

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

