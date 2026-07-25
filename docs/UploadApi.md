# UploadApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botGetUploadUrl**](UploadApi.md#botGetUploadUrl) | **POST** /v1/bot/upload/url | Generate a presigned upload URL |


<a id="botGetUploadUrl"></a>
# **botGetUploadUrl**
> BotGetUploadUrl200Response botGetUploadUrl(botGetUploadUrlRequest)

Generate a presigned upload URL

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = UploadApi()
val botGetUploadUrlRequest : BotGetUploadUrlRequest =  // BotGetUploadUrlRequest | 
try {
    val result : BotGetUploadUrl200Response = apiInstance.botGetUploadUrl(botGetUploadUrlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UploadApi#botGetUploadUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UploadApi#botGetUploadUrl")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **botGetUploadUrlRequest** | [**BotGetUploadUrlRequest**](BotGetUploadUrlRequest.md)|  | |

### Return type

[**BotGetUploadUrl200Response**](BotGetUploadUrl200Response.md)

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

