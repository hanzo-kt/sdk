# APIKeysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteApiKeysByid**](APIKeysApi.md#chatDeleteApiKeysByid) | **DELETE** /v1/chat/api-keys/{id} | Delete an API key |
| [**chatGetApiKeys**](APIKeysApi.md#chatGetApiKeys) | **GET** /v1/chat/api-keys | List agent API keys |
| [**chatGetApiKeysByid**](APIKeysApi.md#chatGetApiKeysByid) | **GET** /v1/chat/api-keys/{id} | Get an API key by ID |
| [**chatPostApiKeys**](APIKeysApi.md#chatPostApiKeys) | **POST** /v1/chat/api-keys | Create an agent API key |


<a id="chatDeleteApiKeysByid"></a>
# **chatDeleteApiKeysByid**
> kotlin.Any chatDeleteApiKeysByid(id)

Delete an API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = APIKeysApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteApiKeysByid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIKeysApi#chatDeleteApiKeysByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIKeysApi#chatDeleteApiKeysByid")
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

<a id="chatGetApiKeys"></a>
# **chatGetApiKeys**
> kotlin.collections.List&lt;ChatAgentApiKey&gt; chatGetApiKeys()

List agent API keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = APIKeysApi()
try {
    val result : kotlin.collections.List<ChatAgentApiKey> = apiInstance.chatGetApiKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIKeysApi#chatGetApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIKeysApi#chatGetApiKeys")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatAgentApiKey&gt;**](ChatAgentApiKey.md)

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

<a id="chatGetApiKeysByid"></a>
# **chatGetApiKeysByid**
> kotlin.Any chatGetApiKeysByid(id)

Get an API key by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = APIKeysApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetApiKeysByid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIKeysApi#chatGetApiKeysByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIKeysApi#chatGetApiKeysByid")
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

<a id="chatPostApiKeys"></a>
# **chatPostApiKeys**
> ChatAgentApiKey chatPostApiKeys(autoCreateTableRequest)

Create an agent API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = APIKeysApi()
val autoCreateTableRequest : AutoCreateTableRequest =  // AutoCreateTableRequest | 
try {
    val result : ChatAgentApiKey = apiInstance.chatPostApiKeys(autoCreateTableRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling APIKeysApi#chatPostApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling APIKeysApi#chatPostApiKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateTableRequest** | [**AutoCreateTableRequest**](AutoCreateTableRequest.md)|  | |

### Return type

[**ChatAgentApiKey**](ChatAgentApiKey.md)

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

