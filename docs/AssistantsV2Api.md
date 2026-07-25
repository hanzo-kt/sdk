# AssistantsV2Api

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteAssistantsV2Byid**](AssistantsV2Api.md#chatDeleteAssistantsV2Byid) | **DELETE** /v1/chat/assistants/v2/{id} | Delete an assistant (v2) |
| [**chatGetAssistantsV2**](AssistantsV2Api.md#chatGetAssistantsV2) | **GET** /v1/chat/assistants/v2 | List assistants (v2) |
| [**chatGetAssistantsV2Byid**](AssistantsV2Api.md#chatGetAssistantsV2Byid) | **GET** /v1/chat/assistants/v2/{id} | Retrieve an assistant (v2) |
| [**chatGetAssistantsV2Documents**](AssistantsV2Api.md#chatGetAssistantsV2Documents) | **GET** /v1/chat/assistants/v2/documents | Get assistant documents (v2) |
| [**chatGetAssistantsV2Tools**](AssistantsV2Api.md#chatGetAssistantsV2Tools) | **GET** /v1/chat/assistants/v2/tools | List available assistant tools (v2) |
| [**chatPatchAssistantsV2Byid**](AssistantsV2Api.md#chatPatchAssistantsV2Byid) | **PATCH** /v1/chat/assistants/v2/{id} | Modify an assistant (v2) |
| [**chatPostAssistantsV2**](AssistantsV2Api.md#chatPostAssistantsV2) | **POST** /v1/chat/assistants/v2 | Create an assistant (v2) |
| [**chatPostAssistantsV2Chat**](AssistantsV2Api.md#chatPostAssistantsV2Chat) | **POST** /v1/chat/assistants/v2/chat | Chat with an assistant (v2) |
| [**chatPostAssistantsV2ChatAbort**](AssistantsV2Api.md#chatPostAssistantsV2ChatAbort) | **POST** /v1/chat/assistants/v2/chat/abort | Abort assistant chat (v2) |


<a id="chatDeleteAssistantsV2Byid"></a>
# **chatDeleteAssistantsV2Byid**
> kotlin.Any chatDeleteAssistantsV2Byid(id)

Delete an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAssistantsV2Byid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatDeleteAssistantsV2Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatDeleteAssistantsV2Byid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="chatGetAssistantsV2"></a>
# **chatGetAssistantsV2**
> kotlin.Any chatGetAssistantsV2()

List assistants (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV2()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatGetAssistantsV2")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatGetAssistantsV2")
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

<a id="chatGetAssistantsV2Byid"></a>
# **chatGetAssistantsV2Byid**
> kotlin.Any chatGetAssistantsV2Byid(id)

Retrieve an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV2Byid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatGetAssistantsV2Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatGetAssistantsV2Byid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="chatGetAssistantsV2Documents"></a>
# **chatGetAssistantsV2Documents**
> kotlin.Any chatGetAssistantsV2Documents()

Get assistant documents (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV2Documents()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatGetAssistantsV2Documents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatGetAssistantsV2Documents")
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

<a id="chatGetAssistantsV2Tools"></a>
# **chatGetAssistantsV2Tools**
> kotlin.Any chatGetAssistantsV2Tools()

List available assistant tools (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV2Tools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatGetAssistantsV2Tools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatGetAssistantsV2Tools")
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

<a id="chatPatchAssistantsV2Byid"></a>
# **chatPatchAssistantsV2Byid**
> kotlin.Any chatPatchAssistantsV2Byid(id, body)

Modify an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPatchAssistantsV2Byid(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatPatchAssistantsV2Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatPatchAssistantsV2Byid")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="chatPostAssistantsV2"></a>
# **chatPostAssistantsV2**
> kotlin.Any chatPostAssistantsV2(body)

Create an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV2(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatPostAssistantsV2")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatPostAssistantsV2")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="chatPostAssistantsV2Chat"></a>
# **chatPostAssistantsV2Chat**
> kotlin.String chatPostAssistantsV2Chat(body)

Chat with an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.String = apiInstance.chatPostAssistantsV2Chat(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatPostAssistantsV2Chat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatPostAssistantsV2Chat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="chatPostAssistantsV2ChatAbort"></a>
# **chatPostAssistantsV2ChatAbort**
> kotlin.Any chatPostAssistantsV2ChatAbort()

Abort assistant chat (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV2Api()
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV2ChatAbort()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV2Api#chatPostAssistantsV2ChatAbort")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV2Api#chatPostAssistantsV2ChatAbort")
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

