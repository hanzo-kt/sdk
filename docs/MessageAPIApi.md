# MessageAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddMessage**](MessageAPIApi.md#cloudApiControllerAddMessage) | **POST** /v1/cloud/add-message | Api Controller Add Message |
| [**cloudApiControllerDeleteMessage**](MessageAPIApi.md#cloudApiControllerDeleteMessage) | **POST** /v1/cloud/delete-message | Api Controller Delete Message |
| [**cloudApiControllerGetAnswer**](MessageAPIApi.md#cloudApiControllerGetAnswer) | **GET** /v1/cloud/get-answer | Api Controller Get Answer |
| [**cloudApiControllerGetGlobalMessages**](MessageAPIApi.md#cloudApiControllerGetGlobalMessages) | **GET** /v1/cloud/get-global-messages | Api Controller Get Global Messages |
| [**cloudApiControllerGetMessage**](MessageAPIApi.md#cloudApiControllerGetMessage) | **GET** /v1/cloud/get-message | Api Controller Get Message |
| [**cloudApiControllerGetMessageAnswer**](MessageAPIApi.md#cloudApiControllerGetMessageAnswer) | **GET** /v1/cloud/get-message-answer | Api Controller Get Message Answer |
| [**cloudApiControllerGetMessages**](MessageAPIApi.md#cloudApiControllerGetMessages) | **GET** /v1/cloud/get-Messages | Api Controller Get Messages |
| [**cloudApiControllerUpdateMessage**](MessageAPIApi.md#cloudApiControllerUpdateMessage) | **POST** /v1/cloud/update-message | Api Controller Update Message |
| [**nexusAddMessage**](MessageAPIApi.md#nexusAddMessage) | **POST** /v1/nexus/add-message | add Message |
| [**nexusDeleteMessage**](MessageAPIApi.md#nexusDeleteMessage) | **POST** /v1/nexus/delete-message | delete Message |
| [**nexusGetAnswer**](MessageAPIApi.md#nexusGetAnswer) | **GET** /v1/nexus/get-answer | get Answer |
| [**nexusGetGlobalMessages**](MessageAPIApi.md#nexusGetGlobalMessages) | **GET** /v1/nexus/get-global-messages | get Global Messages |
| [**nexusGetMessage**](MessageAPIApi.md#nexusGetMessage) | **GET** /v1/nexus/get-message | get Message |
| [**nexusGetMessageAnswer**](MessageAPIApi.md#nexusGetMessageAnswer) | **GET** /v1/nexus/get-message-answer | get Message Answer |
| [**nexusGetMessages**](MessageAPIApi.md#nexusGetMessages) | **GET** /v1/nexus/get-Messages | get Messages |
| [**nexusUpdateMessage**](MessageAPIApi.md#nexusUpdateMessage) | **POST** /v1/nexus/update-message | update Message |


<a id="cloudApiControllerAddMessage"></a>
# **cloudApiControllerAddMessage**
> CloudObjectChat cloudApiControllerAddMessage(cloudObjectMessage)

Api Controller Add Message

add message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val cloudObjectMessage : CloudObjectMessage =  // CloudObjectMessage | The details of the message
try {
    val result : CloudObjectChat = apiInstance.cloudApiControllerAddMessage(cloudObjectMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerAddMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerAddMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMessage** | [**CloudObjectMessage**](CloudObjectMessage.md)| The details of the message | |

### Return type

[**CloudObjectChat**](CloudObjectChat.md)

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

<a id="cloudApiControllerDeleteMessage"></a>
# **cloudApiControllerDeleteMessage**
> CloudControllersResponse cloudApiControllerDeleteMessage(cloudObjectMessage)

Api Controller Delete Message

delete message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val cloudObjectMessage : CloudObjectMessage =  // CloudObjectMessage | The details of the message
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteMessage(cloudObjectMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerDeleteMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerDeleteMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMessage** | [**CloudObjectMessage**](CloudObjectMessage.md)| The details of the message | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetAnswer"></a>
# **cloudApiControllerGetAnswer**
> kotlin.Any cloudApiControllerGetAnswer(provider, question, framework, video)

Api Controller Get Answer

get answer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val provider : kotlin.String = provider_example // kotlin.String | The provider
val question : kotlin.String = question_example // kotlin.String | The question of message
val framework : kotlin.String = framework_example // kotlin.String | The framework
val video : kotlin.String = video_example // kotlin.String | The video
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetAnswer(provider, question, framework, video)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerGetAnswer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerGetAnswer")
    e.printStackTrace()
}
```

### Parameters
| **provider** | **kotlin.String**| The provider | |
| **question** | **kotlin.String**| The question of message | |
| **framework** | **kotlin.String**| The framework | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **video** | **kotlin.String**| The video | |

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

<a id="cloudApiControllerGetGlobalMessages"></a>
# **cloudApiControllerGetGlobalMessages**
> kotlin.collections.List&lt;CloudObjectMessage&gt; cloudApiControllerGetGlobalMessages()

Api Controller Get Global Messages

get global messages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectMessage> = apiInstance.cloudApiControllerGetGlobalMessages()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerGetGlobalMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerGetGlobalMessages")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectMessage&gt;**](CloudObjectMessage.md)

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

<a id="cloudApiControllerGetMessage"></a>
# **cloudApiControllerGetMessage**
> CloudObjectMessage cloudApiControllerGetMessage(id)

Api Controller Get Message

get message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of message
try {
    val result : CloudObjectMessage = apiInstance.cloudApiControllerGetMessage(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerGetMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerGetMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of message | |

### Return type

[**CloudObjectMessage**](CloudObjectMessage.md)

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

<a id="cloudApiControllerGetMessageAnswer"></a>
# **cloudApiControllerGetMessageAnswer**
> kotlin.Any cloudApiControllerGetMessageAnswer(id)

Api Controller Get Message Answer

get message answer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of message
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetMessageAnswer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerGetMessageAnswer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerGetMessageAnswer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of message | |

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

<a id="cloudApiControllerGetMessages"></a>
# **cloudApiControllerGetMessages**
> kotlin.collections.List&lt;CloudObjectMessage&gt; cloudApiControllerGetMessages(user, chat)

Api Controller Get Messages

get Messages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val user : kotlin.String = user_example // kotlin.String | The user of message
val chat : kotlin.String = chat_example // kotlin.String | The chat of message
try {
    val result : kotlin.collections.List<CloudObjectMessage> = apiInstance.cloudApiControllerGetMessages(user, chat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerGetMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerGetMessages")
    e.printStackTrace()
}
```

### Parameters
| **user** | **kotlin.String**| The user of message | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chat** | **kotlin.String**| The chat of message | |

### Return type

[**kotlin.collections.List&lt;CloudObjectMessage&gt;**](CloudObjectMessage.md)

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

<a id="cloudApiControllerUpdateMessage"></a>
# **cloudApiControllerUpdateMessage**
> CloudControllersResponse cloudApiControllerUpdateMessage(id, cloudObjectMessage)

Api Controller Update Message

update message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the message
val cloudObjectMessage : CloudObjectMessage =  // CloudObjectMessage | The details of the message
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateMessage(id, cloudObjectMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#cloudApiControllerUpdateMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#cloudApiControllerUpdateMessage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the message | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMessage** | [**CloudObjectMessage**](CloudObjectMessage.md)| The details of the message | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddMessage"></a>
# **nexusAddMessage**
> CloudObjectChat nexusAddMessage(nexusMessage)

add Message

Add a message to a chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val nexusMessage : NexusMessage =  // NexusMessage | The details of the message
try {
    val result : CloudObjectChat = apiInstance.nexusAddMessage(nexusMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusAddMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusAddMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusMessage** | [**NexusMessage**](NexusMessage.md)| The details of the message | |

### Return type

[**CloudObjectChat**](CloudObjectChat.md)

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

<a id="nexusDeleteMessage"></a>
# **nexusDeleteMessage**
> NexusResponse nexusDeleteMessage(nexusMessage)

delete Message

Delete a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val nexusMessage : NexusMessage =  // NexusMessage | The details of the message
try {
    val result : NexusResponse = apiInstance.nexusDeleteMessage(nexusMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusDeleteMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusDeleteMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusMessage** | [**NexusMessage**](NexusMessage.md)| The details of the message | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetAnswer"></a>
# **nexusGetAnswer**
> kotlin.String nexusGetAnswer(provider, question, framework, video)

get Answer

Get an AI-generated answer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val provider : kotlin.String = provider_example // kotlin.String | The provider
val question : kotlin.String = question_example // kotlin.String | The question
val framework : kotlin.String = framework_example // kotlin.String | The framework
val video : kotlin.String = video_example // kotlin.String | The video
try {
    val result : kotlin.String = apiInstance.nexusGetAnswer(provider, question, framework, video)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusGetAnswer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusGetAnswer")
    e.printStackTrace()
}
```

### Parameters
| **provider** | **kotlin.String**| The provider | |
| **question** | **kotlin.String**| The question | |
| **framework** | **kotlin.String**| The framework | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **video** | **kotlin.String**| The video | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="nexusGetGlobalMessages"></a>
# **nexusGetGlobalMessages**
> kotlin.collections.List&lt;NexusMessage&gt; nexusGetGlobalMessages()

get Global Messages

Get global messages

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
try {
    val result : kotlin.collections.List<NexusMessage> = apiInstance.nexusGetGlobalMessages()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusGetGlobalMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusGetGlobalMessages")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusMessage&gt;**](NexusMessage.md)

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

<a id="nexusGetMessage"></a>
# **nexusGetMessage**
> NexusMessage nexusGetMessage(id)

get Message

Get a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the message
try {
    val result : NexusMessage = apiInstance.nexusGetMessage(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusGetMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusGetMessage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the message | |

### Return type

[**NexusMessage**](NexusMessage.md)

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

<a id="nexusGetMessageAnswer"></a>
# **nexusGetMessageAnswer**
> kotlin.String nexusGetMessageAnswer(id)

get Message Answer

Get a streamed AI answer for a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the message
try {
    val result : kotlin.String = apiInstance.nexusGetMessageAnswer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusGetMessageAnswer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusGetMessageAnswer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the message | |

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

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="nexusGetMessages"></a>
# **nexusGetMessages**
> kotlin.collections.List&lt;NexusMessage&gt; nexusGetMessages(user, chat)

get Messages

Get messages for a chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val user : kotlin.String = user_example // kotlin.String | The user of the messages
val chat : kotlin.String = chat_example // kotlin.String | The chat of the messages
try {
    val result : kotlin.collections.List<NexusMessage> = apiInstance.nexusGetMessages(user, chat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusGetMessages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusGetMessages")
    e.printStackTrace()
}
```

### Parameters
| **user** | **kotlin.String**| The user of the messages | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chat** | **kotlin.String**| The chat of the messages | |

### Return type

[**kotlin.collections.List&lt;NexusMessage&gt;**](NexusMessage.md)

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

<a id="nexusUpdateMessage"></a>
# **nexusUpdateMessage**
> NexusResponse nexusUpdateMessage(id, nexusMessage)

update Message

Update a message

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MessageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the message
val nexusMessage : NexusMessage =  // NexusMessage | The details of the message
try {
    val result : NexusResponse = apiInstance.nexusUpdateMessage(id, nexusMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MessageAPIApi#nexusUpdateMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MessageAPIApi#nexusUpdateMessage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the message | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusMessage** | [**NexusMessage**](NexusMessage.md)| The details of the message | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

