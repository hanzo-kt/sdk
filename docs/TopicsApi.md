# TopicsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**streamCreateTopic**](TopicsApi.md#streamCreateTopic) | **POST** /v1/stream/topics | Create a topic |
| [**streamDeleteTopic**](TopicsApi.md#streamDeleteTopic) | **DELETE** /v1/stream/topics/{topic} | Delete a topic |
| [**streamGetTopicMetadata**](TopicsApi.md#streamGetTopicMetadata) | **GET** /v1/stream/topics/{topic} | Get topic metadata |
| [**streamListTopics**](TopicsApi.md#streamListTopics) | **GET** /v1/stream/topics | List topics |


<a id="streamCreateTopic"></a>
# **streamCreateTopic**
> StreamTopic streamCreateTopic(streamCreateTopicRequest)

Create a topic

Create a new Kafka topic. Under the hood, this creates one PubSub JetStream stream per partition. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TopicsApi()
val streamCreateTopicRequest : StreamCreateTopicRequest = {"name":"events","partitions":3,"replication_factor":1} // StreamCreateTopicRequest | 
try {
    val result : StreamTopic = apiInstance.streamCreateTopic(streamCreateTopicRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TopicsApi#streamCreateTopic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TopicsApi#streamCreateTopic")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **streamCreateTopicRequest** | [**StreamCreateTopicRequest**](StreamCreateTopicRequest.md)|  | |

### Return type

[**StreamTopic**](StreamTopic.md)

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

<a id="streamDeleteTopic"></a>
# **streamDeleteTopic**
> streamDeleteTopic(topic)

Delete a topic

Delete a topic and all associated JetStream streams.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TopicsApi()
val topic : kotlin.String = topic_example // kotlin.String | 
try {
    apiInstance.streamDeleteTopic(topic)
} catch (e: ClientException) {
    println("4xx response calling TopicsApi#streamDeleteTopic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TopicsApi#streamDeleteTopic")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **topic** | **kotlin.String**|  | |

### Return type

null (empty response body)

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

<a id="streamGetTopicMetadata"></a>
# **streamGetTopicMetadata**
> StreamTopicMetadata streamGetTopicMetadata(topic)

Get topic metadata

Returns topic configuration and partition details.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TopicsApi()
val topic : kotlin.String = topic_example // kotlin.String | 
try {
    val result : StreamTopicMetadata = apiInstance.streamGetTopicMetadata(topic)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TopicsApi#streamGetTopicMetadata")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TopicsApi#streamGetTopicMetadata")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **topic** | **kotlin.String**|  | |

### Return type

[**StreamTopicMetadata**](StreamTopicMetadata.md)

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

<a id="streamListTopics"></a>
# **streamListTopics**
> StreamListTopics200Response streamListTopics()

List topics

List all Kafka topics managed by Hanzo Stream.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TopicsApi()
try {
    val result : StreamListTopics200Response = apiInstance.streamListTopics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TopicsApi#streamListTopics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TopicsApi#streamListTopics")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StreamListTopics200Response**](StreamListTopics200Response.md)

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

