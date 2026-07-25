# ChatApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayCreateChatCompletion**](ChatApi.md#gatewayCreateChatCompletion) | **POST** /v1/gateway/chat/completions | Create chat completion |


<a id="gatewayCreateChatCompletion"></a>
# **gatewayCreateChatCompletion**
> GatewayChatCompletionResponse gatewayCreateChatCompletion(gatewayChatCompletionRequest)

Create chat completion

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatApi()
val gatewayChatCompletionRequest : GatewayChatCompletionRequest =  // GatewayChatCompletionRequest | 
try {
    val result : GatewayChatCompletionResponse = apiInstance.gatewayCreateChatCompletion(gatewayChatCompletionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatApi#gatewayCreateChatCompletion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatApi#gatewayCreateChatCompletion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayChatCompletionRequest** | [**GatewayChatCompletionRequest**](GatewayChatCompletionRequest.md)|  | |

### Return type

[**GatewayChatCompletionResponse**](GatewayChatCompletionResponse.md)

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

