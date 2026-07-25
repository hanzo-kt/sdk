# AiApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformAiSuggest**](AiApi.md#platformAiSuggest) | **POST** /v1/platform/ai/suggest | Get AI deployment suggestions |


<a id="platformAiSuggest"></a>
# **platformAiSuggest**
> PlatformTRPCResult platformAiSuggest(platformAiSuggestRequest)

Get AI deployment suggestions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AiApi()
val platformAiSuggestRequest : PlatformAiSuggestRequest =  // PlatformAiSuggestRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformAiSuggest(platformAiSuggestRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiApi#platformAiSuggest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiApi#platformAiSuggest")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformAiSuggestRequest** | [**PlatformAiSuggestRequest**](PlatformAiSuggestRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

