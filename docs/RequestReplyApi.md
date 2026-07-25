# RequestReplyApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pubsubRequestReply**](RequestReplyApi.md#pubsubRequestReply) | **POST** /v1/pubsub/request | Request/reply |


<a id="pubsubRequestReply"></a>
# **pubsubRequestReply**
> PubsubMessage pubsubRequestReply(pubsubPublishRequest, timeout)

Request/reply

Send a request and wait for a reply with timeout.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RequestReplyApi()
val pubsubPublishRequest : PubsubPublishRequest =  // PubsubPublishRequest | 
val timeout : kotlin.Int = 56 // kotlin.Int | Timeout in milliseconds
try {
    val result : PubsubMessage = apiInstance.pubsubRequestReply(pubsubPublishRequest, timeout)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RequestReplyApi#pubsubRequestReply")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RequestReplyApi#pubsubRequestReply")
    e.printStackTrace()
}
```

### Parameters
| **pubsubPublishRequest** | [**PubsubPublishRequest**](PubsubPublishRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timeout** | **kotlin.Int**| Timeout in milliseconds | [optional] [default to 5000] |

### Return type

[**PubsubMessage**](PubsubMessage.md)

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

