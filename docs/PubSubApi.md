# PubSubApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kvListChannels**](PubSubApi.md#kvListChannels) | **GET** /v1/kv/pubsub/channels | List active channels |
| [**kvPublish**](PubSubApi.md#kvPublish) | **POST** /v1/kv/pubsub/publish | Publish message to channel |
| [**kvSubscribe**](PubSubApi.md#kvSubscribe) | **GET** /v1/kv/pubsub/subscribe | Subscribe to channels (SSE) |


<a id="kvListChannels"></a>
# **kvListChannels**
> KvListChannels200Response kvListChannels(pattern)

List active channels

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PubSubApi()
val pattern : kotlin.String = pattern_example // kotlin.String | 
try {
    val result : KvListChannels200Response = apiInstance.kvListChannels(pattern)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PubSubApi#kvListChannels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PubSubApi#kvListChannels")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pattern** | **kotlin.String**|  | [optional] [default to &quot;*&quot;] |

### Return type

[**KvListChannels200Response**](KvListChannels200Response.md)

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

<a id="kvPublish"></a>
# **kvPublish**
> KvPublish200Response kvPublish(kvPublishRequest)

Publish message to channel

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PubSubApi()
val kvPublishRequest : KvPublishRequest =  // KvPublishRequest | 
try {
    val result : KvPublish200Response = apiInstance.kvPublish(kvPublishRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PubSubApi#kvPublish")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PubSubApi#kvPublish")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvPublishRequest** | [**KvPublishRequest**](KvPublishRequest.md)|  | |

### Return type

[**KvPublish200Response**](KvPublish200Response.md)

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

<a id="kvSubscribe"></a>
# **kvSubscribe**
> kotlin.String kvSubscribe(channels, pattern)

Subscribe to channels (SSE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PubSubApi()
val channels : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Channels to subscribe to
val pattern : kotlin.String = pattern_example // kotlin.String | Pattern to subscribe to (e.g. user:*)
try {
    val result : kotlin.String = apiInstance.kvSubscribe(channels, pattern)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PubSubApi#kvSubscribe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PubSubApi#kvSubscribe")
    e.printStackTrace()
}
```

### Parameters
| **channels** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Channels to subscribe to | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pattern** | **kotlin.String**| Pattern to subscribe to (e.g. user:*) | [optional] |

### Return type

**kotlin.String**

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
 - **Accept**: Not defined

