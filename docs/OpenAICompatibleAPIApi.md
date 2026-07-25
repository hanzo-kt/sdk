# OpenAICompatibleAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**nexusChatCompletions**](OpenAICompatibleAPIApi.md#nexusChatCompletions) | **POST** /v1/nexus/chat/completions | chat Completions |


<a id="nexusChatCompletions"></a>
# **nexusChatCompletions**
> kotlin.Any nexusChatCompletions(body)

chat Completions

OpenAI-compatible chat completions endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The OpenAI chat request
try {
    val result : kotlin.Any = apiInstance.nexusChatCompletions(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleAPIApi#nexusChatCompletions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleAPIApi#nexusChatCompletions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The OpenAI chat request | |

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

