# StreamsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kvStreamAdd**](StreamsApi.md#kvStreamAdd) | **POST** /v1/kv/streams/{key}/add | Add entry to stream |
| [**kvStreamInfo**](StreamsApi.md#kvStreamInfo) | **GET** /v1/kv/streams/{key}/info | Get stream info |
| [**kvStreamRead**](StreamsApi.md#kvStreamRead) | **GET** /v1/kv/streams/{key} | Read stream entries |
| [**mqCreateStream**](StreamsApi.md#mqCreateStream) | **POST** /v1/mq/streams | Create stream |
| [**mqDeleteStream**](StreamsApi.md#mqDeleteStream) | **DELETE** /v1/mq/streams/{name} | Delete stream |
| [**mqDeleteStreamMessage**](StreamsApi.md#mqDeleteStreamMessage) | **DELETE** /v1/mq/streams/{name}/messages/{seq} | Delete specific message |
| [**mqGetStream**](StreamsApi.md#mqGetStream) | **GET** /v1/mq/streams/{name} | Get stream info |
| [**mqGetStreamMessages**](StreamsApi.md#mqGetStreamMessages) | **GET** /v1/mq/streams/{name}/messages | Get stream messages |
| [**mqListStreams**](StreamsApi.md#mqListStreams) | **GET** /v1/mq/streams | List streams |
| [**mqPurgeStream**](StreamsApi.md#mqPurgeStream) | **POST** /v1/mq/streams/{name}/purge | Purge stream messages |
| [**mqUpdateStream**](StreamsApi.md#mqUpdateStream) | **PUT** /v1/mq/streams/{name} | Update stream config |
| [**pubsubCreateStream**](StreamsApi.md#pubsubCreateStream) | **POST** /v1/pubsub/jetstream/streams | Create a stream |
| [**pubsubDeleteStream**](StreamsApi.md#pubsubDeleteStream) | **DELETE** /v1/pubsub/jetstream/streams/{stream} | Delete a stream |
| [**pubsubGetStream**](StreamsApi.md#pubsubGetStream) | **GET** /v1/pubsub/jetstream/streams/{stream} | Get stream info |
| [**pubsubListStreams**](StreamsApi.md#pubsubListStreams) | **GET** /v1/pubsub/jetstream/streams | List streams |
| [**pubsubUpdateStream**](StreamsApi.md#pubsubUpdateStream) | **PUT** /v1/pubsub/jetstream/streams/{stream} | Update stream config |


<a id="kvStreamAdd"></a>
# **kvStreamAdd**
> KvStreamAdd201Response kvStreamAdd(key, kvStreamAddRequest, namespace)

Add entry to stream

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val key : kotlin.String = key_example // kotlin.String | 
val kvStreamAddRequest : KvStreamAddRequest =  // KvStreamAddRequest | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvStreamAdd201Response = apiInstance.kvStreamAdd(key, kvStreamAddRequest, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#kvStreamAdd")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#kvStreamAdd")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **kvStreamAddRequest** | [**KvStreamAddRequest**](KvStreamAddRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvStreamAdd201Response**](KvStreamAdd201Response.md)

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

<a id="kvStreamInfo"></a>
# **kvStreamInfo**
> KvStreamInfo200Response kvStreamInfo(key, namespace)

Get stream info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val key : kotlin.String = key_example // kotlin.String | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvStreamInfo200Response = apiInstance.kvStreamInfo(key, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#kvStreamInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#kvStreamInfo")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvStreamInfo200Response**](KvStreamInfo200Response.md)

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

<a id="kvStreamRead"></a>
# **kvStreamRead**
> KvStreamRead200Response kvStreamRead(key, start, end, count, namespace)

Read stream entries

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val key : kotlin.String = key_example // kotlin.String | 
val start : kotlin.String = start_example // kotlin.String | Start ID (- for beginning)
val end : kotlin.String = end_example // kotlin.String | End ID (+ for latest)
val count : kotlin.Int = 56 // kotlin.Int | 
val namespace : kotlin.String = namespace_example // kotlin.String | 
try {
    val result : KvStreamRead200Response = apiInstance.kvStreamRead(key, start, end, count, namespace)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#kvStreamRead")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#kvStreamRead")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| **start** | **kotlin.String**| Start ID (- for beginning) | [optional] [default to &quot;-&quot;] |
| **end** | **kotlin.String**| End ID (+ for latest) | [optional] [default to &quot;+&quot;] |
| **count** | **kotlin.Int**|  | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **namespace** | **kotlin.String**|  | [optional] |

### Return type

[**KvStreamRead200Response**](KvStreamRead200Response.md)

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

<a id="mqCreateStream"></a>
# **mqCreateStream**
> MqStream mqCreateStream(mqStreamConfig)

Create stream

Creates a new JetStream stream with the specified configuration. Streams provide durable, replicated message storage with configurable retention policies. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val mqStreamConfig : MqStreamConfig =  // MqStreamConfig | 
try {
    val result : MqStream = apiInstance.mqCreateStream(mqStreamConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqCreateStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqCreateStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqStreamConfig** | [**MqStreamConfig**](MqStreamConfig.md)|  | |

### Return type

[**MqStream**](MqStream.md)

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

<a id="mqDeleteStream"></a>
# **mqDeleteStream**
> mqDeleteStream(name)

Delete stream

Deletes a stream and all its messages and consumers. This operation is irreversible. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
try {
    apiInstance.mqDeleteStream(name)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqDeleteStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqDeleteStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Stream name. | |

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

<a id="mqDeleteStreamMessage"></a>
# **mqDeleteStreamMessage**
> mqDeleteStreamMessage(name, seq)

Delete specific message

Deletes a specific message from the stream by sequence number. The sequence gap remains; subsequent messages are not renumbered. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
val seq : kotlin.Int = 56 // kotlin.Int | Message sequence number.
try {
    apiInstance.mqDeleteStreamMessage(name, seq)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqDeleteStreamMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqDeleteStreamMessage")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **seq** | **kotlin.Int**| Message sequence number. | |

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

<a id="mqGetStream"></a>
# **mqGetStream**
> MqStream mqGetStream(name)

Get stream info

Returns stream configuration and current state including message count, byte size, and consumer count. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
try {
    val result : MqStream = apiInstance.mqGetStream(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqGetStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqGetStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Stream name. | |

### Return type

[**MqStream**](MqStream.md)

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

<a id="mqGetStreamMessages"></a>
# **mqGetStreamMessages**
> MqGetStreamMessages200Response mqGetStreamMessages(name, seq, lastBySubject, nextBySubject, limit)

Get stream messages

Retrieves messages from the stream by sequence number or subject. Use for direct message access without a consumer. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
val seq : kotlin.Int = 56 // kotlin.Int | Get message at this sequence number.
val lastBySubject : kotlin.String = lastBySubject_example // kotlin.String | Get last message for the given subject.
val nextBySubject : kotlin.String = nextBySubject_example // kotlin.String | Get next message for the given subject (requires seq param as starting point). 
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
try {
    val result : MqGetStreamMessages200Response = apiInstance.mqGetStreamMessages(name, seq, lastBySubject, nextBySubject, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqGetStreamMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqGetStreamMessages")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Stream name. | |
| **seq** | **kotlin.Int**| Get message at this sequence number. | [optional] |
| **lastBySubject** | **kotlin.String**| Get last message for the given subject. | [optional] |
| **nextBySubject** | **kotlin.String**| Get next message for the given subject (requires seq param as starting point).  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="mqListStreams"></a>
# **mqListStreams**
> MqListStreams200Response mqListStreams(limit, offset)

List streams

Returns all JetStream streams for the authenticated account.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListStreams200Response = apiInstance.mqListStreams(limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqListStreams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqListStreams")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListStreams200Response**](MqListStreams200Response.md)

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

<a id="mqPurgeStream"></a>
# **mqPurgeStream**
> MqPurgeStream200Response mqPurgeStream(name, mqPurgeStreamRequest)

Purge stream messages

Removes all messages from the stream. Consumers are not deleted. Optionally filter by subject to purge only matching messages. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
val mqPurgeStreamRequest : MqPurgeStreamRequest =  // MqPurgeStreamRequest | 
try {
    val result : MqPurgeStream200Response = apiInstance.mqPurgeStream(name, mqPurgeStreamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqPurgeStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqPurgeStream")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqPurgeStreamRequest** | [**MqPurgeStreamRequest**](MqPurgeStreamRequest.md)|  | [optional] |

### Return type

[**MqPurgeStream200Response**](MqPurgeStream200Response.md)

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

<a id="mqUpdateStream"></a>
# **mqUpdateStream**
> MqStream mqUpdateStream(name, mqStreamConfig)

Update stream config

Updates an existing stream&#39;s configuration. Not all fields are mutable after creation (e.g., storage type cannot change). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val name : kotlin.String = name_example // kotlin.String | Stream name.
val mqStreamConfig : MqStreamConfig =  // MqStreamConfig | 
try {
    val result : MqStream = apiInstance.mqUpdateStream(name, mqStreamConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#mqUpdateStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#mqUpdateStream")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Stream name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mqStreamConfig** | [**MqStreamConfig**](MqStreamConfig.md)|  | |

### Return type

[**MqStream**](MqStream.md)

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

<a id="pubsubCreateStream"></a>
# **pubsubCreateStream**
> PubsubStreamInfo pubsubCreateStream(pubsubStreamConfig)

Create a stream

Create a new JetStream stream for persistent message storage.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val pubsubStreamConfig : PubsubStreamConfig = {"name":"ORDERS","subjects":["orders.>"],"storage":"file","replicas":3,"retention":"limits","max_age":86400000000000} // PubsubStreamConfig | 
try {
    val result : PubsubStreamInfo = apiInstance.pubsubCreateStream(pubsubStreamConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#pubsubCreateStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#pubsubCreateStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pubsubStreamConfig** | [**PubsubStreamConfig**](PubsubStreamConfig.md)|  | |

### Return type

[**PubsubStreamInfo**](PubsubStreamInfo.md)

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

<a id="pubsubDeleteStream"></a>
# **pubsubDeleteStream**
> pubsubDeleteStream(stream)

Delete a stream

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val stream : kotlin.String = stream_example // kotlin.String | 
try {
    apiInstance.pubsubDeleteStream(stream)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#pubsubDeleteStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#pubsubDeleteStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stream** | **kotlin.String**|  | |

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

<a id="pubsubGetStream"></a>
# **pubsubGetStream**
> PubsubStreamInfo pubsubGetStream(stream)

Get stream info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val stream : kotlin.String = stream_example // kotlin.String | 
try {
    val result : PubsubStreamInfo = apiInstance.pubsubGetStream(stream)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#pubsubGetStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#pubsubGetStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stream** | **kotlin.String**|  | |

### Return type

[**PubsubStreamInfo**](PubsubStreamInfo.md)

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

<a id="pubsubListStreams"></a>
# **pubsubListStreams**
> PubsubListStreams200Response pubsubListStreams()

List streams

List all JetStream streams.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
try {
    val result : PubsubListStreams200Response = apiInstance.pubsubListStreams()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#pubsubListStreams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#pubsubListStreams")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PubsubListStreams200Response**](PubsubListStreams200Response.md)

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

<a id="pubsubUpdateStream"></a>
# **pubsubUpdateStream**
> PubsubStreamInfo pubsubUpdateStream(stream, pubsubStreamConfig)

Update stream config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StreamsApi()
val stream : kotlin.String = stream_example // kotlin.String | 
val pubsubStreamConfig : PubsubStreamConfig =  // PubsubStreamConfig | 
try {
    val result : PubsubStreamInfo = apiInstance.pubsubUpdateStream(stream, pubsubStreamConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamsApi#pubsubUpdateStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamsApi#pubsubUpdateStream")
    e.printStackTrace()
}
```

### Parameters
| **stream** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pubsubStreamConfig** | [**PubsubStreamConfig**](PubsubStreamConfig.md)|  | |

### Return type

[**PubsubStreamInfo**](PubsubStreamInfo.md)

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

