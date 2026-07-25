# MediaApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleGetMedia**](MediaApi.md#consoleGetMedia) | **GET** /v1/console/media/{mediaId} | Get a media record |
| [**consoleGetMediaUploadUrl**](MediaApi.md#consoleGetMediaUploadUrl) | **POST** /v1/console/media | Get a presigned upload URL for a media record |
| [**consolePatchMedia**](MediaApi.md#consolePatchMedia) | **PATCH** /v1/console/media/{mediaId} | Patch a media record (update upload status) |


<a id="consoleGetMedia"></a>
# **consoleGetMedia**
> ConsoleMediaRecord consoleGetMedia(mediaId)

Get a media record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MediaApi()
val mediaId : kotlin.String = mediaId_example // kotlin.String | 
try {
    val result : ConsoleMediaRecord = apiInstance.consoleGetMedia(mediaId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MediaApi#consoleGetMedia")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MediaApi#consoleGetMedia")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mediaId** | **kotlin.String**|  | |

### Return type

[**ConsoleMediaRecord**](ConsoleMediaRecord.md)

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

<a id="consoleGetMediaUploadUrl"></a>
# **consoleGetMediaUploadUrl**
> ConsoleGetMediaUploadUrl200Response consoleGetMediaUploadUrl(consoleGetMediaUploadUrlRequest)

Get a presigned upload URL for a media record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MediaApi()
val consoleGetMediaUploadUrlRequest : ConsoleGetMediaUploadUrlRequest =  // ConsoleGetMediaUploadUrlRequest | 
try {
    val result : ConsoleGetMediaUploadUrl200Response = apiInstance.consoleGetMediaUploadUrl(consoleGetMediaUploadUrlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MediaApi#consoleGetMediaUploadUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MediaApi#consoleGetMediaUploadUrl")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleGetMediaUploadUrlRequest** | [**ConsoleGetMediaUploadUrlRequest**](ConsoleGetMediaUploadUrlRequest.md)|  | |

### Return type

[**ConsoleGetMediaUploadUrl200Response**](ConsoleGetMediaUploadUrl200Response.md)

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

<a id="consolePatchMedia"></a>
# **consolePatchMedia**
> consolePatchMedia(mediaId, consolePatchMediaRequest)

Patch a media record (update upload status)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MediaApi()
val mediaId : kotlin.String = mediaId_example // kotlin.String | 
val consolePatchMediaRequest : ConsolePatchMediaRequest =  // ConsolePatchMediaRequest | 
try {
    apiInstance.consolePatchMedia(mediaId, consolePatchMediaRequest)
} catch (e: ClientException) {
    println("4xx response calling MediaApi#consolePatchMedia")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MediaApi#consolePatchMedia")
    e.printStackTrace()
}
```

### Parameters
| **mediaId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consolePatchMediaRequest** | [**ConsolePatchMediaRequest**](ConsolePatchMediaRequest.md)|  | |

### Return type

null (empty response body)

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

