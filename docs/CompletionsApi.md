# CompletionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayCreateCompletion**](CompletionsApi.md#gatewayCreateCompletion) | **POST** /v1/gateway/completions | Create completion |


<a id="gatewayCreateCompletion"></a>
# **gatewayCreateCompletion**
> kotlin.Any gatewayCreateCompletion(gatewayCreateCompletionRequest)

Create completion

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompletionsApi()
val gatewayCreateCompletionRequest : GatewayCreateCompletionRequest =  // GatewayCreateCompletionRequest | 
try {
    val result : kotlin.Any = apiInstance.gatewayCreateCompletion(gatewayCreateCompletionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CompletionsApi#gatewayCreateCompletion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompletionsApi#gatewayCreateCompletion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayCreateCompletionRequest** | [**GatewayCreateCompletionRequest**](GatewayCreateCompletionRequest.md)|  | |

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

