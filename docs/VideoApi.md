# VideoApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldYoutubeEmbed**](VideoApi.md#worldWorldYoutubeEmbed) | **GET** /v1/world/youtube/embed | Self-contained IFrame-API player page (text/html) |
| [**worldWorldYoutubeLive**](VideoApi.md#worldWorldYoutubeLive) | **GET** /v1/world/youtube/live | Resolve a channel handle to its current LIVE video id |


<a id="worldWorldYoutubeEmbed"></a>
# **worldWorldYoutubeEmbed**
> kotlin.String worldWorldYoutubeEmbed(videoId)

Self-contained IFrame-API player page (text/html)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoApi()
val videoId : kotlin.String = videoId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.worldWorldYoutubeEmbed(videoId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoApi#worldWorldYoutubeEmbed")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoApi#worldWorldYoutubeEmbed")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **videoId** | **kotlin.String**|  | |

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

<a id="worldWorldYoutubeLive"></a>
# **worldWorldYoutubeLive**
> kotlin.Any worldWorldYoutubeLive(channel)

Resolve a channel handle to its current LIVE video id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoApi()
val channel : kotlin.String = channel_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldYoutubeLive(channel)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoApi#worldWorldYoutubeLive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoApi#worldWorldYoutubeLive")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **channel** | **kotlin.String**|  | |

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

