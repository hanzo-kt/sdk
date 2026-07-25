# ConsumersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqCreateConsumer**](ConsumersApi.md#mqCreateConsumer) | **POST** /v1/mq/streams/{stream}/consumers | Create consumer |
| [**mqDeleteConsumer**](ConsumersApi.md#mqDeleteConsumer) | **DELETE** /v1/mq/streams/{stream}/consumers/{name} | Delete consumer |
| [**mqGetConsumer**](ConsumersApi.md#mqGetConsumer) | **GET** /v1/mq/streams/{stream}/consumers/{name} | Get consumer info |
| [**mqListConsumers**](ConsumersApi.md#mqListConsumers) | **GET** /v1/mq/streams/{stream}/consumers | List consumers |
| [**mqPullMessages**](ConsumersApi.md#mqPullMessages) | **POST** /v1/mq/streams/{stream}/consumers/{name}/next | Pull next message(s) |
| [**pubsubCreateConsumer**](ConsumersApi.md#pubsubCreateConsumer) | **POST** /v1/pubsub/jetstream/streams/{stream}/consumers | Create a consumer |
| [**pubsubDeleteConsumer**](ConsumersApi.md#pubsubDeleteConsumer) | **DELETE** /v1/pubsub/jetstream/streams/{stream}/consumers/{consumer} | Delete a consumer |
| [**pubsubGetConsumer**](ConsumersApi.md#pubsubGetConsumer) | **GET** /v1/pubsub/jetstream/streams/{stream}/consumers/{consumer} | Get consumer info |
| [**pubsubListConsumers**](ConsumersApi.md#pubsubListConsumers) | **GET** /v1/pubsub/jetstream/streams/{stream}/consumers | List consumers |


<a id="mqCreateConsumer"></a>
# **mqCreateConsumer**
> MqConsumer mqCreateConsumer(stream, mqConsumerConfig)

Create consumer

Creates a new consumer on the specified stream. Consumers track delivery state and support at-least-once or exactly-once semantics depending on the ack policy. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | Stream name.
val mqConsumerConfig : MqConsumerConfig =  // MqConsumerConfig | 
try {
    val result : MqConsumer = apiInstance.mqCreateConsumer(stream, mqConsumerConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#mqCreateConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#mqCreateConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqConsumerConfig** | [**MqConsumerConfig**](MqConsumerConfig.md)|  | |

### Return type

[**MqConsumer**](MqConsumer.md)

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

<a id="mqDeleteConsumer"></a>
# **mqDeleteConsumer**
> mqDeleteConsumer(stream, name)

Delete consumer

Deletes a consumer and its delivery state. Unacknowledged messages remain in the stream. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | Stream name.
val name : kotlin.String = name_example // kotlin.String | Consumer name.
try {
    apiInstance.mqDeleteConsumer(stream, name)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#mqDeleteConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#mqDeleteConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Consumer name. | |

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
 - **Accept**: application/json

<a id="mqGetConsumer"></a>
# **mqGetConsumer**
> MqConsumer mqGetConsumer(stream, name)

Get consumer info

Returns consumer configuration and delivery state including pending count, ack floor, and redelivery metrics. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | Stream name.
val name : kotlin.String = name_example // kotlin.String | Consumer name.
try {
    val result : MqConsumer = apiInstance.mqGetConsumer(stream, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#mqGetConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#mqGetConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Consumer name. | |

### Return type

[**MqConsumer**](MqConsumer.md)

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

<a id="mqListConsumers"></a>
# **mqListConsumers**
> MqListConsumers200Response mqListConsumers(stream, limit, offset)

List consumers

Returns all consumers for the specified stream.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | Stream name.
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListConsumers200Response = apiInstance.mqListConsumers(stream, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#mqListConsumers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#mqListConsumers")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**| Stream name. | |
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListConsumers200Response**](MqListConsumers200Response.md)

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

<a id="mqPullMessages"></a>
# **mqPullMessages**
> MqGetStreamMessages200Response mqPullMessages(stream, name, mqPullMessagesRequest)

Pull next message(s)

Pulls the next batch of messages from the consumer. Supports configurable batch size, timeout, and no-wait mode. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | Stream name.
val name : kotlin.String = name_example // kotlin.String | Consumer name.
val mqPullMessagesRequest : MqPullMessagesRequest =  // MqPullMessagesRequest | 
try {
    val result : MqGetStreamMessages200Response = apiInstance.mqPullMessages(stream, name, mqPullMessagesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#mqPullMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#mqPullMessages")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**| Stream name. | |
| **name** | **kotlin.String**| Consumer name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqPullMessagesRequest** | [**MqPullMessagesRequest**](MqPullMessagesRequest.md)|  | [optional] |

### Return type

[**MqGetStreamMessages200Response**](MqGetStreamMessages200Response.md)

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

<a id="pubsubCreateConsumer"></a>
# **pubsubCreateConsumer**
> PubsubConsumerInfo pubsubCreateConsumer(stream, pubsubConsumerConfig)

Create a consumer

Create a durable or ephemeral consumer on a stream.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | 
val pubsubConsumerConfig : PubsubConsumerConfig = {"durable_name":"order-processor","ack_policy":"explicit","filter_subject":"orders.created"} // PubsubConsumerConfig | 
try {
    val result : PubsubConsumerInfo = apiInstance.pubsubCreateConsumer(stream, pubsubConsumerConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#pubsubCreateConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#pubsubCreateConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pubsubConsumerConfig** | [**PubsubConsumerConfig**](PubsubConsumerConfig.md)|  | |

### Return type

[**PubsubConsumerInfo**](PubsubConsumerInfo.md)

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

<a id="pubsubDeleteConsumer"></a>
# **pubsubDeleteConsumer**
> pubsubDeleteConsumer(stream, consumer)

Delete a consumer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | 
val consumer : kotlin.String = consumer_example // kotlin.String | 
try {
    apiInstance.pubsubDeleteConsumer(stream, consumer)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#pubsubDeleteConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#pubsubDeleteConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consumer** | **kotlin.String**|  | |

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

<a id="pubsubGetConsumer"></a>
# **pubsubGetConsumer**
> PubsubConsumerInfo pubsubGetConsumer(stream, consumer)

Get consumer info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | 
val consumer : kotlin.String = consumer_example // kotlin.String | 
try {
    val result : PubsubConsumerInfo = apiInstance.pubsubGetConsumer(stream, consumer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#pubsubGetConsumer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#pubsubGetConsumer")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consumer** | **kotlin.String**|  | |

### Return type

[**PubsubConsumerInfo**](PubsubConsumerInfo.md)

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

<a id="pubsubListConsumers"></a>
# **pubsubListConsumers**
> PubsubListConsumers200Response pubsubListConsumers(stream)

List consumers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumersApi()
val stream : kotlin.String = stream_example // kotlin.String | 
try {
    val result : PubsubListConsumers200Response = apiInstance.pubsubListConsumers(stream)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumersApi#pubsubListConsumers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumersApi#pubsubListConsumers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stream** | **kotlin.String**|  | |

### Return type

[**PubsubListConsumers200Response**](PubsubListConsumers200Response.md)

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

