# PresetsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetPresets**](PresetsApi.md#chatGetPresets) | **GET** /v1/chat/presets | List user presets |
| [**chatPostPresets**](PresetsApi.md#chatPostPresets) | **POST** /v1/chat/presets | Create or update a preset |
| [**chatPostPresetsDelete**](PresetsApi.md#chatPostPresetsDelete) | **POST** /v1/chat/presets/delete | Delete a preset |


<a id="chatGetPresets"></a>
# **chatGetPresets**
> kotlin.collections.List&lt;ChatPreset&gt; chatGetPresets()

List user presets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PresetsApi()
try {
    val result : kotlin.collections.List<ChatPreset> = apiInstance.chatGetPresets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PresetsApi#chatGetPresets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PresetsApi#chatGetPresets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatPreset&gt;**](ChatPreset.md)

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

<a id="chatPostPresets"></a>
# **chatPostPresets**
> ChatPreset chatPostPresets(chatPreset)

Create or update a preset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PresetsApi()
val chatPreset : ChatPreset =  // ChatPreset | 
try {
    val result : ChatPreset = apiInstance.chatPostPresets(chatPreset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PresetsApi#chatPostPresets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PresetsApi#chatPostPresets")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPreset** | [**ChatPreset**](ChatPreset.md)|  | |

### Return type

[**ChatPreset**](ChatPreset.md)

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

<a id="chatPostPresetsDelete"></a>
# **chatPostPresetsDelete**
> kotlin.Any chatPostPresetsDelete(chatPostPresetsDeleteRequest)

Delete a preset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PresetsApi()
val chatPostPresetsDeleteRequest : ChatPostPresetsDeleteRequest =  // ChatPostPresetsDeleteRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostPresetsDelete(chatPostPresetsDeleteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PresetsApi#chatPostPresetsDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PresetsApi#chatPostPresetsDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostPresetsDeleteRequest** | [**ChatPostPresetsDeleteRequest**](ChatPostPresetsDeleteRequest.md)|  | [optional] |

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

