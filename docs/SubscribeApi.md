# SubscribeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqSubscribe**](SubscribeApi.md#mqSubscribe) | **GET** /v1/mq/subscribe/{subject} | Subscribe to subject via SSE |
| [**pubsubSubscribe**](SubscribeApi.md#pubsubSubscribe) | **GET** /v1/pubsub/subscribe | Subscribe to a subject (SSE) |


<a id="mqSubscribe"></a>
# **mqSubscribe**
> MqMessage mqSubscribe(subject, queue)

Subscribe to subject via SSE

Opens a Server-Sent Events stream for messages on the given subject. Supports NATS wildcard tokens: &#x60;*&#x60; matches a single token, &#x60;&gt;&#x60; matches one or more tokens. The connection stays open until the client disconnects. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscribeApi()
val subject : kotlin.String = subject_example // kotlin.String | Subject to subscribe to. Supports wildcards (`events.*`, `logs.>`). 
val queue : kotlin.String = queue_example // kotlin.String | Queue group name for load-balanced delivery.
try {
    val result : MqMessage = apiInstance.mqSubscribe(subject, queue)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscribeApi#mqSubscribe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscribeApi#mqSubscribe")
    e.printStackTrace()
}
```

### Parameters
| **subject** | **kotlin.String**| Subject to subscribe to. Supports wildcards (&#x60;events.*&#x60;, &#x60;logs.&gt;&#x60;).  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **queue** | **kotlin.String**| Queue group name for load-balanced delivery. | [optional] |

### Return type

[**MqMessage**](MqMessage.md)

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

<a id="pubsubSubscribe"></a>
# **pubsubSubscribe**
> PubsubMessage pubsubSubscribe(subject, queue)

Subscribe to a subject (SSE)

Subscribe to messages on a subject using Server-Sent Events. Supports wildcard subscriptions (&#x60;&gt;&#x60; for multi-level, &#x60;*&#x60; for single-level). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscribeApi()
val subject : kotlin.String = orders.> // kotlin.String | Subject to subscribe to (supports wildcards)
val queue : kotlin.String = queue_example // kotlin.String | Queue group name for load-balanced delivery
try {
    val result : PubsubMessage = apiInstance.pubsubSubscribe(subject, queue)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscribeApi#pubsubSubscribe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscribeApi#pubsubSubscribe")
    e.printStackTrace()
}
```

### Parameters
| **subject** | **kotlin.String**| Subject to subscribe to (supports wildcards) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **queue** | **kotlin.String**| Queue group name for load-balanced delivery | [optional] |

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

 - **Content-Type**: Not defined
 - **Accept**: Not defined

