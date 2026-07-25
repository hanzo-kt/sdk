# AssistantsV1Api

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteAssistantsV1Byid**](AssistantsV1Api.md#chatDeleteAssistantsV1Byid) | **DELETE** /v1/chat/assistants/v1/{id} | Delete an assistant (v1) |
| [**chatGetAssistantsV1**](AssistantsV1Api.md#chatGetAssistantsV1) | **GET** /v1/chat/assistants/v1 | List assistants (v1) |
| [**chatGetAssistantsV1Byid**](AssistantsV1Api.md#chatGetAssistantsV1Byid) | **GET** /v1/chat/assistants/v1/{id} | Retrieve an assistant (v1) |
| [**chatGetAssistantsV1Documents**](AssistantsV1Api.md#chatGetAssistantsV1Documents) | **GET** /v1/chat/assistants/v1/documents | Get assistant documents |
| [**chatGetAssistantsV1Tools**](AssistantsV1Api.md#chatGetAssistantsV1Tools) | **GET** /v1/chat/assistants/v1/tools | List available assistant tools |
| [**chatPatchAssistantsV1Byid**](AssistantsV1Api.md#chatPatchAssistantsV1Byid) | **PATCH** /v1/chat/assistants/v1/{id} | Modify an assistant (v1) |
| [**chatPostAssistantsV1**](AssistantsV1Api.md#chatPostAssistantsV1) | **POST** /v1/chat/assistants/v1 | Create an assistant (v1) |
| [**chatPostAssistantsV1Chat**](AssistantsV1Api.md#chatPostAssistantsV1Chat) | **POST** /v1/chat/assistants/v1/chat | Chat with an assistant (v1) |
| [**chatPostAssistantsV1ChatAbort**](AssistantsV1Api.md#chatPostAssistantsV1ChatAbort) | **POST** /v1/chat/assistants/v1/chat/abort | Abort assistant chat (v1) |


<a id="chatDeleteAssistantsV1Byid"></a>
# **chatDeleteAssistantsV1Byid**
> kotlin.Any chatDeleteAssistantsV1Byid(id)

Delete an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAssistantsV1Byid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatDeleteAssistantsV1Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatDeleteAssistantsV1Byid")
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

<a id="chatGetAssistantsV1"></a>
# **chatGetAssistantsV1**
> kotlin.Any chatGetAssistantsV1()

List assistants (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV1()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatGetAssistantsV1")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatGetAssistantsV1")
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

<a id="chatGetAssistantsV1Byid"></a>
# **chatGetAssistantsV1Byid**
> kotlin.Any chatGetAssistantsV1Byid(id)

Retrieve an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV1Byid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatGetAssistantsV1Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatGetAssistantsV1Byid")
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

<a id="chatGetAssistantsV1Documents"></a>
# **chatGetAssistantsV1Documents**
> kotlin.Any chatGetAssistantsV1Documents()

Get assistant documents

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV1Documents()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatGetAssistantsV1Documents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatGetAssistantsV1Documents")
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

<a id="chatGetAssistantsV1Tools"></a>
# **chatGetAssistantsV1Tools**
> kotlin.Any chatGetAssistantsV1Tools()

List available assistant tools

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
try {
    val result : kotlin.Any = apiInstance.chatGetAssistantsV1Tools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatGetAssistantsV1Tools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatGetAssistantsV1Tools")
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

<a id="chatPatchAssistantsV1Byid"></a>
# **chatPatchAssistantsV1Byid**
> kotlin.Any chatPatchAssistantsV1Byid(id, body)

Modify an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPatchAssistantsV1Byid(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatPatchAssistantsV1Byid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatPatchAssistantsV1Byid")
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

<a id="chatPostAssistantsV1"></a>
# **chatPostAssistantsV1**
> kotlin.Any chatPostAssistantsV1(body)

Create an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV1(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatPostAssistantsV1")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatPostAssistantsV1")
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

<a id="chatPostAssistantsV1Chat"></a>
# **chatPostAssistantsV1Chat**
> kotlin.String chatPostAssistantsV1Chat(body)

Chat with an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.String = apiInstance.chatPostAssistantsV1Chat(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatPostAssistantsV1Chat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatPostAssistantsV1Chat")
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

<a id="chatPostAssistantsV1ChatAbort"></a>
# **chatPostAssistantsV1ChatAbort**
> kotlin.Any chatPostAssistantsV1ChatAbort()

Abort assistant chat (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AssistantsV1Api()
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV1ChatAbort()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AssistantsV1Api#chatPostAssistantsV1ChatAbort")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AssistantsV1Api#chatPostAssistantsV1ChatAbort")
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

