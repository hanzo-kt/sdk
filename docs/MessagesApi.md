# MessagesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteMessagesByconversationidBymessageid**](MessagesApi.md#chatDeleteMessagesByconversationidBymessageid) | **DELETE** /v1/chat/messages/{conversationId}/{messageId} | Delete a message |
| [**chatGetMessages**](MessagesApi.md#chatGetMessages) | **GET** /v1/chat/messages | Query messages |
| [**chatGetMessagesByconversationid**](MessagesApi.md#chatGetMessagesByconversationid) | **GET** /v1/chat/messages/{conversationId} | Get all messages in a conversation |
| [**chatGetMessagesByconversationidBymessageid**](MessagesApi.md#chatGetMessagesByconversationidBymessageid) | **GET** /v1/chat/messages/{conversationId}/{messageId} | Get a specific message |
| [**chatPostMessagesArtifactBymessageid**](MessagesApi.md#chatPostMessagesArtifactBymessageid) | **POST** /v1/chat/messages/artifact/{messageId} | Edit artifact content in a message |
| [**chatPostMessagesBranch**](MessagesApi.md#chatPostMessagesBranch) | **POST** /v1/chat/messages/branch | Create a branch message |
| [**chatPostMessagesByconversationid**](MessagesApi.md#chatPostMessagesByconversationid) | **POST** /v1/chat/messages/{conversationId} | Save a message to a conversation |
| [**chatPutMessagesByconversationidBymessageid**](MessagesApi.md#chatPutMessagesByconversationidBymessageid) | **PUT** /v1/chat/messages/{conversationId}/{messageId} | Update a message |
| [**chatPutMessagesByconversationidBymessageidFeedback**](MessagesApi.md#chatPutMessagesByconversationidBymessageidFeedback) | **PUT** /v1/chat/messages/{conversationId}/{messageId}/feedback | Update message feedback |
| [**streamConsumeMessages**](MessagesApi.md#streamConsumeMessages) | **GET** /v1/stream/topics/{topic}/messages | Consume messages |
| [**streamProduceMessages**](MessagesApi.md#streamProduceMessages) | **POST** /v1/stream/topics/{topic}/messages | Produce messages |


<a id="chatDeleteMessagesByconversationidBymessageid"></a>
# **chatDeleteMessagesByconversationidBymessageid**
> chatDeleteMessagesByconversationidBymessageid(conversationId, messageId)

Delete a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val messageId : kotlin.String = messageId_example // kotlin.String | 
try {
    apiInstance.chatDeleteMessagesByconversationidBymessageid(conversationId, messageId)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatDeleteMessagesByconversationidBymessageid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatDeleteMessagesByconversationidBymessageid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **messageId** | **kotlin.String**|  | |

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

<a id="chatGetMessages"></a>
# **chatGetMessages**
> ChatGetMessages200Response chatGetMessages(conversationId, messageId, search, cursor, pageSize, sortBy, sortDirection)

Query messages

Search messages or retrieve by conversation/message ID.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val messageId : kotlin.String = messageId_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val sortDirection : kotlin.String = sortDirection_example // kotlin.String | 
try {
    val result : ChatGetMessages200Response = apiInstance.chatGetMessages(conversationId, messageId, search, cursor, pageSize, sortBy, sortDirection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatGetMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatGetMessages")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | [optional] |
| **messageId** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 25] |
| **sortBy** | **kotlin.String**|  | [optional] [default to &quot;createdAt&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sortDirection** | **kotlin.String**|  | [optional] [default to &quot;desc&quot;] |

### Return type

[**ChatGetMessages200Response**](ChatGetMessages200Response.md)

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

<a id="chatGetMessagesByconversationid"></a>
# **chatGetMessagesByconversationid**
> kotlin.collections.List&lt;ChatMessage&gt; chatGetMessagesByconversationid(conversationId)

Get all messages in a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ChatMessage> = apiInstance.chatGetMessagesByconversationid(conversationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatGetMessagesByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatGetMessagesByconversationid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conversationId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;ChatMessage&gt;**](ChatMessage.md)

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

<a id="chatGetMessagesByconversationidBymessageid"></a>
# **chatGetMessagesByconversationidBymessageid**
> ChatMessage chatGetMessagesByconversationidBymessageid(conversationId, messageId)

Get a specific message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val messageId : kotlin.String = messageId_example // kotlin.String | 
try {
    val result : ChatMessage = apiInstance.chatGetMessagesByconversationidBymessageid(conversationId, messageId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatGetMessagesByconversationidBymessageid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatGetMessagesByconversationidBymessageid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **messageId** | **kotlin.String**|  | |

### Return type

[**ChatMessage**](ChatMessage.md)

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

<a id="chatPostMessagesArtifactBymessageid"></a>
# **chatPostMessagesArtifactBymessageid**
> ChatPostMessagesArtifactBymessageid200Response chatPostMessagesArtifactBymessageid(messageId, chatPostMessagesArtifactBymessageidRequest)

Edit artifact content in a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val messageId : kotlin.String = messageId_example // kotlin.String | 
val chatPostMessagesArtifactBymessageidRequest : ChatPostMessagesArtifactBymessageidRequest =  // ChatPostMessagesArtifactBymessageidRequest | 
try {
    val result : ChatPostMessagesArtifactBymessageid200Response = apiInstance.chatPostMessagesArtifactBymessageid(messageId, chatPostMessagesArtifactBymessageidRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatPostMessagesArtifactBymessageid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatPostMessagesArtifactBymessageid")
    e.printStackTrace()
}
```

### Parameters
| **messageId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostMessagesArtifactBymessageidRequest** | [**ChatPostMessagesArtifactBymessageidRequest**](ChatPostMessagesArtifactBymessageidRequest.md)|  | |

### Return type

[**ChatPostMessagesArtifactBymessageid200Response**](ChatPostMessagesArtifactBymessageid200Response.md)

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

<a id="chatPostMessagesBranch"></a>
# **chatPostMessagesBranch**
> ChatMessage chatPostMessagesBranch(chatPostMessagesBranchRequest)

Create a branch message

Branch a specific agent&#39;s content from a parallel response message.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val chatPostMessagesBranchRequest : ChatPostMessagesBranchRequest =  // ChatPostMessagesBranchRequest | 
try {
    val result : ChatMessage = apiInstance.chatPostMessagesBranch(chatPostMessagesBranchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatPostMessagesBranch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatPostMessagesBranch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostMessagesBranchRequest** | [**ChatPostMessagesBranchRequest**](ChatPostMessagesBranchRequest.md)|  | |

### Return type

[**ChatMessage**](ChatMessage.md)

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

<a id="chatPostMessagesByconversationid"></a>
# **chatPostMessagesByconversationid**
> ChatMessage chatPostMessagesByconversationid(conversationId, chatMessage)

Save a message to a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val chatMessage : ChatMessage =  // ChatMessage | 
try {
    val result : ChatMessage = apiInstance.chatPostMessagesByconversationid(conversationId, chatMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatPostMessagesByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatPostMessagesByconversationid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatMessage** | [**ChatMessage**](ChatMessage.md)|  | |

### Return type

[**ChatMessage**](ChatMessage.md)

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

<a id="chatPutMessagesByconversationidBymessageid"></a>
# **chatPutMessagesByconversationidBymessageid**
> kotlin.Any chatPutMessagesByconversationidBymessageid(conversationId, messageId, chatPutMessagesByconversationidBymessageidRequest)

Update a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val messageId : kotlin.String = messageId_example // kotlin.String | 
val chatPutMessagesByconversationidBymessageidRequest : ChatPutMessagesByconversationidBymessageidRequest =  // ChatPutMessagesByconversationidBymessageidRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPutMessagesByconversationidBymessageid(conversationId, messageId, chatPutMessagesByconversationidBymessageidRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatPutMessagesByconversationidBymessageid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatPutMessagesByconversationidBymessageid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| **messageId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPutMessagesByconversationidBymessageidRequest** | [**ChatPutMessagesByconversationidBymessageidRequest**](ChatPutMessagesByconversationidBymessageidRequest.md)|  | |

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

<a id="chatPutMessagesByconversationidBymessageidFeedback"></a>
# **chatPutMessagesByconversationidBymessageidFeedback**
> ChatPutMessagesByconversationidBymessageidFeedback200Response chatPutMessagesByconversationidBymessageidFeedback(conversationId, messageId, chatPutMessagesByconversationidBymessageidFeedbackRequest)

Update message feedback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val messageId : kotlin.String = messageId_example // kotlin.String | 
val chatPutMessagesByconversationidBymessageidFeedbackRequest : ChatPutMessagesByconversationidBymessageidFeedbackRequest =  // ChatPutMessagesByconversationidBymessageidFeedbackRequest | 
try {
    val result : ChatPutMessagesByconversationidBymessageidFeedback200Response = apiInstance.chatPutMessagesByconversationidBymessageidFeedback(conversationId, messageId, chatPutMessagesByconversationidBymessageidFeedbackRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#chatPutMessagesByconversationidBymessageidFeedback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#chatPutMessagesByconversationidBymessageidFeedback")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| **messageId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPutMessagesByconversationidBymessageidFeedbackRequest** | [**ChatPutMessagesByconversationidBymessageidFeedbackRequest**](ChatPutMessagesByconversationidBymessageidFeedbackRequest.md)|  | |

### Return type

[**ChatPutMessagesByconversationidBymessageidFeedback200Response**](ChatPutMessagesByconversationidBymessageidFeedback200Response.md)

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

<a id="streamConsumeMessages"></a>
# **streamConsumeMessages**
> StreamConsumeMessages200Response streamConsumeMessages(topic, partition, offset, limit, timeout)

Consume messages

Consume messages from a topic partition via REST API. For persistent consumption, use the Kafka wire protocol with consumer groups. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val topic : kotlin.String = topic_example // kotlin.String | 
val partition : kotlin.Int = 56 // kotlin.Int | Partition to consume from
val offset : kotlin.String = offset_example // kotlin.String | Starting offset (earliest, latest, or numeric offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum records to return
val timeout : kotlin.Int = 56 // kotlin.Int | Long-poll timeout in milliseconds
try {
    val result : StreamConsumeMessages200Response = apiInstance.streamConsumeMessages(topic, partition, offset, limit, timeout)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#streamConsumeMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#streamConsumeMessages")
    e.printStackTrace()
}
```

### Parameters
| **topic** | **kotlin.String**|  | |
| **partition** | **kotlin.Int**| Partition to consume from | [optional] [default to 0] |
| **offset** | **kotlin.String**| Starting offset (earliest, latest, or numeric offset) | [optional] [default to &quot;latest&quot;] |
| **limit** | **kotlin.Int**| Maximum records to return | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timeout** | **kotlin.Int**| Long-poll timeout in milliseconds | [optional] [default to 5000] |

### Return type

[**StreamConsumeMessages200Response**](StreamConsumeMessages200Response.md)

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

<a id="streamProduceMessages"></a>
# **streamProduceMessages**
> StreamProduceResponse streamProduceMessages(topic, streamProduceRequest)

Produce messages

Produce one or more messages to a topic via REST API. For high throughput, use the Kafka wire protocol on port 9092. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessagesApi()
val topic : kotlin.String = topic_example // kotlin.String | 
val streamProduceRequest : StreamProduceRequest = {"records":[{"value":"{\"event\":\"user.signup\",\"user_id\":\"usr_123\"}"}]} // StreamProduceRequest | 
try {
    val result : StreamProduceResponse = apiInstance.streamProduceMessages(topic, streamProduceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessagesApi#streamProduceMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessagesApi#streamProduceMessages")
    e.printStackTrace()
}
```

### Parameters
| **topic** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **streamProduceRequest** | [**StreamProduceRequest**](StreamProduceRequest.md)|  | |

### Return type

[**StreamProduceResponse**](StreamProduceResponse.md)

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

