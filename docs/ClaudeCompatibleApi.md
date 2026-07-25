# ClaudeCompatibleApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aiCreateMessage**](ClaudeCompatibleApi.md#aiCreateMessage) | **POST** /v1/messages | Create a message (Anthropic-compatible) |


<a id="aiCreateMessage"></a>
# **aiCreateMessage**
> AiMessageResponse aiCreateMessage(aiMessageRequest)

Create a message (Anthropic-compatible)

Anthropic Messages-compatible endpoint. Set &#x60;stream: true&#x60; for an SSE event stream. Drop-in for the Anthropic SDK and Claude Code&#39;s &#x60;ANTHROPIC_BASE_URL&#x60;. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClaudeCompatibleApi()
val aiMessageRequest : AiMessageRequest =  // AiMessageRequest | 
try {
    val result : AiMessageResponse = apiInstance.aiCreateMessage(aiMessageRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClaudeCompatibleApi#aiCreateMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClaudeCompatibleApi#aiCreateMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiMessageRequest** | [**AiMessageRequest**](AiMessageRequest.md)|  | |

### Return type

[**AiMessageResponse**](AiMessageResponse.md)

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

