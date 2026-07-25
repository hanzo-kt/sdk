# MemoriesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteMemoriesBykey**](MemoriesApi.md#chatDeleteMemoriesBykey) | **DELETE** /v1/chat/memories/{key} | Delete a memory |
| [**chatGetMemories**](MemoriesApi.md#chatGetMemories) | **GET** /v1/chat/memories | Get all user memories |
| [**chatPatchMemoriesBykey**](MemoriesApi.md#chatPatchMemoriesBykey) | **PATCH** /v1/chat/memories/{key} | Update a memory |
| [**chatPatchMemoriesPreferences**](MemoriesApi.md#chatPatchMemoriesPreferences) | **PATCH** /v1/chat/memories/preferences | Update memory preferences |
| [**chatPostMemories**](MemoriesApi.md#chatPostMemories) | **POST** /v1/chat/memories | Create a memory |


<a id="chatDeleteMemoriesBykey"></a>
# **chatDeleteMemoriesBykey**
> kotlin.Any chatDeleteMemoriesBykey(key)

Delete a memory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MemoriesApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteMemoriesBykey(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MemoriesApi#chatDeleteMemoriesBykey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MemoriesApi#chatDeleteMemoriesBykey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="chatGetMemories"></a>
# **chatGetMemories**
> ChatGetMemories200Response chatGetMemories()

Get all user memories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MemoriesApi()
try {
    val result : ChatGetMemories200Response = apiInstance.chatGetMemories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MemoriesApi#chatGetMemories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MemoriesApi#chatGetMemories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetMemories200Response**](ChatGetMemories200Response.md)

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

<a id="chatPatchMemoriesBykey"></a>
# **chatPatchMemoriesBykey**
> kotlin.Any chatPatchMemoriesBykey(key, chatPatchMemoriesBykeyRequest)

Update a memory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MemoriesApi()
val key : kotlin.String = key_example // kotlin.String | 
val chatPatchMemoriesBykeyRequest : ChatPatchMemoriesBykeyRequest =  // ChatPatchMemoriesBykeyRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPatchMemoriesBykey(key, chatPatchMemoriesBykeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MemoriesApi#chatPatchMemoriesBykey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MemoriesApi#chatPatchMemoriesBykey")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPatchMemoriesBykeyRequest** | [**ChatPatchMemoriesBykeyRequest**](ChatPatchMemoriesBykeyRequest.md)|  | |

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

<a id="chatPatchMemoriesPreferences"></a>
# **chatPatchMemoriesPreferences**
> kotlin.Any chatPatchMemoriesPreferences(chatPatchMemoriesPreferencesRequest)

Update memory preferences

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MemoriesApi()
val chatPatchMemoriesPreferencesRequest : ChatPatchMemoriesPreferencesRequest =  // ChatPatchMemoriesPreferencesRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPatchMemoriesPreferences(chatPatchMemoriesPreferencesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MemoriesApi#chatPatchMemoriesPreferences")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MemoriesApi#chatPatchMemoriesPreferences")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPatchMemoriesPreferencesRequest** | [**ChatPatchMemoriesPreferencesRequest**](ChatPatchMemoriesPreferencesRequest.md)|  | |

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

<a id="chatPostMemories"></a>
# **chatPostMemories**
> ChatPostMemories201Response chatPostMemories(chatPostMemoriesRequest)

Create a memory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MemoriesApi()
val chatPostMemoriesRequest : ChatPostMemoriesRequest =  // ChatPostMemoriesRequest | 
try {
    val result : ChatPostMemories201Response = apiInstance.chatPostMemories(chatPostMemoriesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MemoriesApi#chatPostMemories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MemoriesApi#chatPostMemories")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostMemoriesRequest** | [**ChatPostMemoriesRequest**](ChatPostMemoriesRequest.md)|  | |

### Return type

[**ChatPostMemories201Response**](ChatPostMemories201Response.md)

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

