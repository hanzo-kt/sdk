# PublishApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqPublishMessage**](PublishApi.md#mqPublishMessage) | **POST** /v1/mq/publish | Publish message to subject |
| [**mqRequestReply**](PublishApi.md#mqRequestReply) | **POST** /v1/mq/request | Request/reply pattern |
| [**pubsubPublishMessage**](PublishApi.md#pubsubPublishMessage) | **POST** /v1/pubsub/publish | Publish a message |


<a id="mqPublishMessage"></a>
# **mqPublishMessage**
> MqPublishResponse mqPublishMessage(mqPublishRequest)

Publish message to subject

Publish a message to the specified subject. Supports optional headers and reply-to subject for request/reply patterns. If the subject is bound to a JetStream stream, the message is persisted. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PublishApi()
val mqPublishRequest : MqPublishRequest =  // MqPublishRequest | 
try {
    val result : MqPublishResponse = apiInstance.mqPublishMessage(mqPublishRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublishApi#mqPublishMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublishApi#mqPublishMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqPublishRequest** | [**MqPublishRequest**](MqPublishRequest.md)|  | |

### Return type

[**MqPublishResponse**](MqPublishResponse.md)

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

<a id="mqRequestReply"></a>
# **mqRequestReply**
> MqMessage mqRequestReply(mqRequestReply)

Request/reply pattern

Publishes a message and waits for a single reply within the specified timeout. Uses an ephemeral inbox subject for the reply. Returns the reply message or a timeout error. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PublishApi()
val mqRequestReply : MqRequestReply =  // MqRequestReply | 
try {
    val result : MqMessage = apiInstance.mqRequestReply(mqRequestReply)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublishApi#mqRequestReply")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublishApi#mqRequestReply")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqRequestReply** | [**MqRequestReply**](MqRequestReply.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="pubsubPublishMessage"></a>
# **pubsubPublishMessage**
> PubsubPublishResponse pubsubPublishMessage(pubsubPublishRequest)

Publish a message

Publish a message to a subject. If the subject is captured by a JetStream stream, the message is durably stored.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PublishApi()
val pubsubPublishRequest : PubsubPublishRequest = {"subject":"orders.created","data":"{\"id\":\"order-123\",\"total\":59.99}"} // PubsubPublishRequest | 
try {
    val result : PubsubPublishResponse = apiInstance.pubsubPublishMessage(pubsubPublishRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublishApi#pubsubPublishMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublishApi#pubsubPublishMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pubsubPublishRequest** | [**PubsubPublishRequest**](PubsubPublishRequest.md)|  | |

### Return type

[**PubsubPublishResponse**](PubsubPublishResponse.md)

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

