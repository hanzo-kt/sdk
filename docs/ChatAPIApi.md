# ChatAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddChat**](ChatAPIApi.md#cloudApiControllerAddChat) | **POST** /v1/cloud/add-chat | Api Controller Add Chat |
| [**cloudApiControllerDeleteChat**](ChatAPIApi.md#cloudApiControllerDeleteChat) | **POST** /v1/cloud/delete-chat | Api Controller Delete Chat |
| [**cloudApiControllerGetChat**](ChatAPIApi.md#cloudApiControllerGetChat) | **GET** /v1/cloud/get-chat | Api Controller Get Chat |
| [**cloudApiControllerGetChats**](ChatAPIApi.md#cloudApiControllerGetChats) | **GET** /v1/cloud/get-chats | Api Controller Get Chats |
| [**cloudApiControllerGetGlobalChats**](ChatAPIApi.md#cloudApiControllerGetGlobalChats) | **GET** /v1/cloud/get-global-chats | Api Controller Get Global Chats |
| [**cloudApiControllerUpdateChat**](ChatAPIApi.md#cloudApiControllerUpdateChat) | **POST** /v1/cloud/update-chat | Api Controller Update Chat |
| [**nexusAddChat**](ChatAPIApi.md#nexusAddChat) | **POST** /v1/nexus/add-chat | add Chat |
| [**nexusDeleteChat**](ChatAPIApi.md#nexusDeleteChat) | **POST** /v1/nexus/delete-chat | delete Chat |
| [**nexusGetChat**](ChatAPIApi.md#nexusGetChat) | **GET** /v1/nexus/get-chat | get Chat |
| [**nexusGetChats**](ChatAPIApi.md#nexusGetChats) | **GET** /v1/nexus/get-chats | get Chats |
| [**nexusGetGlobalChats**](ChatAPIApi.md#nexusGetGlobalChats) | **GET** /v1/nexus/get-global-chats | get Global Chats |
| [**nexusUpdateChat**](ChatAPIApi.md#nexusUpdateChat) | **POST** /v1/nexus/update-chat | update Chat |


<a id="cloudApiControllerAddChat"></a>
# **cloudApiControllerAddChat**
> CloudControllersResponse cloudApiControllerAddChat(cloudObjectChat)

Api Controller Add Chat

add chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddChat(cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerAddChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerAddChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

<a id="cloudApiControllerDeleteChat"></a>
# **cloudApiControllerDeleteChat**
> CloudControllersResponse cloudApiControllerDeleteChat(cloudObjectChat)

Api Controller Delete Chat

delete chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteChat(cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerDeleteChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerDeleteChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

<a id="cloudApiControllerGetChat"></a>
# **cloudApiControllerGetChat**
> CloudObjectChat cloudApiControllerGetChat(id)

Api Controller Get Chat

get chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of chat
try {
    val result : CloudObjectChat = apiInstance.cloudApiControllerGetChat(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerGetChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerGetChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of chat | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="cloudApiControllerGetChats"></a>
# **cloudApiControllerGetChats**
> kotlin.collections.List&lt;CloudObjectChat&gt; cloudApiControllerGetChats(user, `field`, `value`)

Api Controller Get Chats

get chats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val user : kotlin.String = user_example // kotlin.String | The user of chat
val `field` : kotlin.String = `field`_example // kotlin.String | The field of chat
val `value` : kotlin.String = `value`_example // kotlin.String | The value of chat
try {
    val result : kotlin.collections.List<CloudObjectChat> = apiInstance.cloudApiControllerGetChats(user, `field`, `value`)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerGetChats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerGetChats")
    e.printStackTrace()
}
```

### Parameters
| **user** | **kotlin.String**| The user of chat | |
| **&#x60;field&#x60;** | **kotlin.String**| The field of chat | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **&#x60;value&#x60;** | **kotlin.String**| The value of chat | |

### Return type

[**kotlin.collections.List&lt;CloudObjectChat&gt;**](CloudObjectChat.md)

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

<a id="cloudApiControllerGetGlobalChats"></a>
# **cloudApiControllerGetGlobalChats**
> kotlin.collections.List&lt;CloudObjectChat&gt; cloudApiControllerGetGlobalChats()

Api Controller Get Global Chats

get global chats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectChat> = apiInstance.cloudApiControllerGetGlobalChats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerGetGlobalChats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerGetGlobalChats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectChat&gt;**](CloudObjectChat.md)

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

<a id="cloudApiControllerUpdateChat"></a>
# **cloudApiControllerUpdateChat**
> CloudControllersResponse cloudApiControllerUpdateChat(id, cloudObjectChat)

Api Controller Update Chat

update Chat

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the chat
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateChat(id, cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#cloudApiControllerUpdateChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#cloudApiControllerUpdateChat")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the chat | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

<a id="nexusAddChat"></a>
# **nexusAddChat**
> NexusResponse nexusAddChat(cloudObjectChat)

add Chat

Add a chat session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : NexusResponse = apiInstance.nexusAddChat(cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusAddChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusAddChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

<a id="nexusDeleteChat"></a>
# **nexusDeleteChat**
> NexusResponse nexusDeleteChat(cloudObjectChat)

delete Chat

Delete a chat session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : NexusResponse = apiInstance.nexusDeleteChat(cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusDeleteChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusDeleteChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

<a id="nexusGetChat"></a>
# **nexusGetChat**
> CloudObjectChat nexusGetChat(id)

get Chat

Get a chat session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the chat
try {
    val result : CloudObjectChat = apiInstance.nexusGetChat(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusGetChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusGetChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the chat | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="nexusGetChats"></a>
# **nexusGetChats**
> kotlin.collections.List&lt;CloudObjectChat&gt; nexusGetChats(user, `field`, `value`)

get Chats

Get chat sessions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val user : kotlin.String = user_example // kotlin.String | The user of the chats
val `field` : kotlin.String = `field`_example // kotlin.String | The field to filter by
val `value` : kotlin.String = `value`_example // kotlin.String | The value to filter by
try {
    val result : kotlin.collections.List<CloudObjectChat> = apiInstance.nexusGetChats(user, `field`, `value`)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusGetChats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusGetChats")
    e.printStackTrace()
}
```

### Parameters
| **user** | **kotlin.String**| The user of the chats | |
| **&#x60;field&#x60;** | **kotlin.String**| The field to filter by | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **&#x60;value&#x60;** | **kotlin.String**| The value to filter by | |

### Return type

[**kotlin.collections.List&lt;CloudObjectChat&gt;**](CloudObjectChat.md)

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

<a id="nexusGetGlobalChats"></a>
# **nexusGetGlobalChats**
> kotlin.collections.List&lt;CloudObjectChat&gt; nexusGetGlobalChats()

get Global Chats

Get global chats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectChat> = apiInstance.nexusGetGlobalChats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusGetGlobalChats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusGetGlobalChats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectChat&gt;**](CloudObjectChat.md)

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

<a id="nexusUpdateChat"></a>
# **nexusUpdateChat**
> NexusResponse nexusUpdateChat(id, cloudObjectChat)

update Chat

Update a chat session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ChatAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the chat
val cloudObjectChat : CloudObjectChat =  // CloudObjectChat | The details of the chat
try {
    val result : NexusResponse = apiInstance.nexusUpdateChat(id, cloudObjectChat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ChatAPIApi#nexusUpdateChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ChatAPIApi#nexusUpdateChat")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the chat | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectChat** | [**CloudObjectChat**](CloudObjectChat.md)| The details of the chat | |

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

