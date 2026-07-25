# TagsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteTagsBytag**](TagsApi.md#chatDeleteTagsBytag) | **DELETE** /v1/chat/tags/{tag} | Delete a conversation tag |
| [**chatGetTags**](TagsApi.md#chatGetTags) | **GET** /v1/chat/tags | Get all conversation tags |
| [**chatPostTags**](TagsApi.md#chatPostTags) | **POST** /v1/chat/tags | Create a conversation tag |
| [**chatPutTagsBytag**](TagsApi.md#chatPutTagsBytag) | **PUT** /v1/chat/tags/{tag} | Update a conversation tag |
| [**chatPutTagsConvoByconversationid**](TagsApi.md#chatPutTagsConvoByconversationid) | **PUT** /v1/chat/tags/convo/{conversationId} | Update tags for a conversation |
| [**flowListTags**](TagsApi.md#flowListTags) | **GET** /v1/flow/tags | List piece tags |


<a id="chatDeleteTagsBytag"></a>
# **chatDeleteTagsBytag**
> kotlin.Any chatDeleteTagsBytag(tag)

Delete a conversation tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
val tag : kotlin.String = tag_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteTagsBytag(tag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#chatDeleteTagsBytag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#chatDeleteTagsBytag")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tag** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatGetTags"></a>
# **chatGetTags**
> kotlin.collections.List&lt;ChatConversationTag&gt; chatGetTags()

Get all conversation tags

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
try {
    val result : kotlin.collections.List<ChatConversationTag> = apiInstance.chatGetTags()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#chatGetTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#chatGetTags")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatConversationTag&gt;**](ChatConversationTag.md)

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

<a id="chatPostTags"></a>
# **chatPostTags**
> kotlin.Any chatPostTags(chatConversationTag)

Create a conversation tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
val chatConversationTag : ChatConversationTag =  // ChatConversationTag | 
try {
    val result : kotlin.Any = apiInstance.chatPostTags(chatConversationTag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#chatPostTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#chatPostTags")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatConversationTag** | [**ChatConversationTag**](ChatConversationTag.md)|  | |

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

<a id="chatPutTagsBytag"></a>
# **chatPutTagsBytag**
> kotlin.Any chatPutTagsBytag(tag, chatConversationTag)

Update a conversation tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
val tag : kotlin.String = tag_example // kotlin.String | 
val chatConversationTag : ChatConversationTag =  // ChatConversationTag | 
try {
    val result : kotlin.Any = apiInstance.chatPutTagsBytag(tag, chatConversationTag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#chatPutTagsBytag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#chatPutTagsBytag")
    e.printStackTrace()
}
```

### Parameters
| **tag** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatConversationTag** | [**ChatConversationTag**](ChatConversationTag.md)|  | |

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

<a id="chatPutTagsConvoByconversationid"></a>
# **chatPutTagsConvoByconversationid**
> kotlin.Any chatPutTagsConvoByconversationid(conversationId, chatPutTagsConvoByconversationidRequest)

Update tags for a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
val chatPutTagsConvoByconversationidRequest : ChatPutTagsConvoByconversationidRequest =  // ChatPutTagsConvoByconversationidRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPutTagsConvoByconversationid(conversationId, chatPutTagsConvoByconversationidRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#chatPutTagsConvoByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#chatPutTagsConvoByconversationid")
    e.printStackTrace()
}
```

### Parameters
| **conversationId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPutTagsConvoByconversationidRequest** | [**ChatPutTagsConvoByconversationidRequest**](ChatPutTagsConvoByconversationidRequest.md)|  | |

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

<a id="flowListTags"></a>
# **flowListTags**
> kotlin.Any flowListTags()

List piece tags

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TagsApi()
try {
    val result : kotlin.Any = apiInstance.flowListTags()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TagsApi#flowListTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TagsApi#flowListTags")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

