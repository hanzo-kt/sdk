# ConversationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteConvos**](ConversationsApi.md#chatDeleteConvos) | **DELETE** /v1/chat/convos | Delete a conversation |
| [**chatDeleteConvosAll**](ConversationsApi.md#chatDeleteConvosAll) | **DELETE** /v1/chat/convos/all | Delete all conversations |
| [**chatGetConvos**](ConversationsApi.md#chatGetConvos) | **GET** /v1/chat/convos | List conversations |
| [**chatGetConvosByconversationid**](ConversationsApi.md#chatGetConvosByconversationid) | **GET** /v1/chat/convos/{conversationId} | Get a conversation |
| [**chatGetConvosGenTitleByconversationid**](ConversationsApi.md#chatGetConvosGenTitleByconversationid) | **GET** /v1/chat/convos/gen_title/{conversationId} | Get generated title for conversation |
| [**chatPostConvosArchive**](ConversationsApi.md#chatPostConvosArchive) | **POST** /v1/chat/convos/archive | Archive or unarchive a conversation |
| [**chatPostConvosDuplicate**](ConversationsApi.md#chatPostConvosDuplicate) | **POST** /v1/chat/convos/duplicate | Duplicate a conversation |
| [**chatPostConvosFork**](ConversationsApi.md#chatPostConvosFork) | **POST** /v1/chat/convos/fork | Fork a conversation |
| [**chatPostConvosImport**](ConversationsApi.md#chatPostConvosImport) | **POST** /v1/chat/convos/import | Import conversations from JSON file |
| [**chatPostConvosUpdate**](ConversationsApi.md#chatPostConvosUpdate) | **POST** /v1/chat/convos/update | Update a conversation title |


<a id="chatDeleteConvos"></a>
# **chatDeleteConvos**
> kotlin.Any chatDeleteConvos(chatDeleteConvosRequest)

Delete a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val chatDeleteConvosRequest : ChatDeleteConvosRequest =  // ChatDeleteConvosRequest | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteConvos(chatDeleteConvosRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatDeleteConvos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatDeleteConvos")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatDeleteConvosRequest** | [**ChatDeleteConvosRequest**](ChatDeleteConvosRequest.md)|  | |

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

<a id="chatDeleteConvosAll"></a>
# **chatDeleteConvosAll**
> kotlin.Any chatDeleteConvosAll()

Delete all conversations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
try {
    val result : kotlin.Any = apiInstance.chatDeleteConvosAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatDeleteConvosAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatDeleteConvosAll")
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

<a id="chatGetConvos"></a>
# **chatGetConvos**
> ChatConversationListResponse chatGetConvos(limit, cursor, isArchived, tags, search, sortBy, sortDirection)

List conversations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val isArchived : kotlin.String = isArchived_example // kotlin.String | 
val tags : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val search : kotlin.String = search_example // kotlin.String | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val sortDirection : kotlin.String = sortDirection_example // kotlin.String | 
try {
    val result : ChatConversationListResponse = apiInstance.chatGetConvos(limit, cursor, isArchived, tags, search, sortBy, sortDirection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatGetConvos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatGetConvos")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**|  | [optional] [default to 25] |
| **cursor** | **kotlin.String**|  | [optional] |
| **isArchived** | **kotlin.String**|  | [optional] |
| **tags** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **sortBy** | **kotlin.String**|  | [optional] [default to &quot;updatedAt&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sortDirection** | **kotlin.String**|  | [optional] [default to &quot;desc&quot;] |

### Return type

[**ChatConversationListResponse**](ChatConversationListResponse.md)

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

<a id="chatGetConvosByconversationid"></a>
# **chatGetConvosByconversationid**
> ChatConversation chatGetConvosByconversationid(conversationId)

Get a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
try {
    val result : ChatConversation = apiInstance.chatGetConvosByconversationid(conversationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatGetConvosByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatGetConvosByconversationid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conversationId** | **kotlin.String**|  | |

### Return type

[**ChatConversation**](ChatConversation.md)

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

<a id="chatGetConvosGenTitleByconversationid"></a>
# **chatGetConvosGenTitleByconversationid**
> ChatGetConvosGenTitleByconversationid200Response chatGetConvosGenTitleByconversationid(conversationId)

Get generated title for conversation

Polls for an AI-generated title. Uses exponential backoff.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
try {
    val result : ChatGetConvosGenTitleByconversationid200Response = apiInstance.chatGetConvosGenTitleByconversationid(conversationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatGetConvosGenTitleByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatGetConvosGenTitleByconversationid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conversationId** | **kotlin.String**|  | |

### Return type

[**ChatGetConvosGenTitleByconversationid200Response**](ChatGetConvosGenTitleByconversationid200Response.md)

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

<a id="chatPostConvosArchive"></a>
# **chatPostConvosArchive**
> ChatConversation chatPostConvosArchive(chatPostConvosArchiveRequest)

Archive or unarchive a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val chatPostConvosArchiveRequest : ChatPostConvosArchiveRequest =  // ChatPostConvosArchiveRequest | 
try {
    val result : ChatConversation = apiInstance.chatPostConvosArchive(chatPostConvosArchiveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatPostConvosArchive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatPostConvosArchive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostConvosArchiveRequest** | [**ChatPostConvosArchiveRequest**](ChatPostConvosArchiveRequest.md)|  | |

### Return type

[**ChatConversation**](ChatConversation.md)

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

<a id="chatPostConvosDuplicate"></a>
# **chatPostConvosDuplicate**
> kotlin.Any chatPostConvosDuplicate(chatPostConvosDuplicateRequest)

Duplicate a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val chatPostConvosDuplicateRequest : ChatPostConvosDuplicateRequest =  // ChatPostConvosDuplicateRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostConvosDuplicate(chatPostConvosDuplicateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatPostConvosDuplicate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatPostConvosDuplicate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostConvosDuplicateRequest** | [**ChatPostConvosDuplicateRequest**](ChatPostConvosDuplicateRequest.md)|  | |

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

<a id="chatPostConvosFork"></a>
# **chatPostConvosFork**
> ChatPostConvosFork200Response chatPostConvosFork(chatPostConvosForkRequest)

Fork a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val chatPostConvosForkRequest : ChatPostConvosForkRequest =  // ChatPostConvosForkRequest | 
try {
    val result : ChatPostConvosFork200Response = apiInstance.chatPostConvosFork(chatPostConvosForkRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatPostConvosFork")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatPostConvosFork")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostConvosForkRequest** | [**ChatPostConvosForkRequest**](ChatPostConvosForkRequest.md)|  | |

### Return type

[**ChatPostConvosFork200Response**](ChatPostConvosFork200Response.md)

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

<a id="chatPostConvosImport"></a>
# **chatPostConvosImport**
> kotlin.Any chatPostConvosImport(file)

Import conversations from JSON file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : kotlin.Any = apiInstance.chatPostConvosImport(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatPostConvosImport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatPostConvosImport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**|  | [optional] |

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

<a id="chatPostConvosUpdate"></a>
# **chatPostConvosUpdate**
> kotlin.Any chatPostConvosUpdate(chatPostConvosUpdateRequest)

Update a conversation title

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConversationsApi()
val chatPostConvosUpdateRequest : ChatPostConvosUpdateRequest =  // ChatPostConvosUpdateRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostConvosUpdate(chatPostConvosUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConversationsApi#chatPostConvosUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConversationsApi#chatPostConvosUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostConvosUpdateRequest** | [**ChatPostConvosUpdateRequest**](ChatPostConvosUpdateRequest.md)|  | |

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

