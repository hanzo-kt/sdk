# STTAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerProcessSpeechToText**](STTAPIApi.md#cloudApiControllerProcessSpeechToText) | **POST** /v1/cloud/process-speech-to-text | Api Controller Process Speech To Text |
| [**nexusProcessSpeechToText**](STTAPIApi.md#nexusProcessSpeechToText) | **POST** /v1/nexus/process-speech-to-text | process Speech To Text |


<a id="cloudApiControllerProcessSpeechToText"></a>
# **cloudApiControllerProcessSpeechToText**
> kotlin.Any cloudApiControllerProcessSpeechToText(audio, storeId)

Api Controller Process Speech To Text

convert speech to text

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = STTAPIApi()
val audio : java.io.File = BINARY_DATA_HERE // java.io.File | The audio file to convert to text
val storeId : kotlin.String = storeId_example // kotlin.String | The store ID
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerProcessSpeechToText(audio, storeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling STTAPIApi#cloudApiControllerProcessSpeechToText")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling STTAPIApi#cloudApiControllerProcessSpeechToText")
    e.printStackTrace()
}
```

### Parameters
| **audio** | **java.io.File**| The audio file to convert to text | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **storeId** | **kotlin.String**| The store ID | |

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

<a id="nexusProcessSpeechToText"></a>
# **nexusProcessSpeechToText**
> kotlin.Any nexusProcessSpeechToText(audio, storeId)

process Speech To Text

Convert speech to text

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = STTAPIApi()
val audio : java.io.File = BINARY_DATA_HERE // java.io.File | The audio file to convert to text
val storeId : kotlin.String = storeId_example // kotlin.String | The store ID
try {
    val result : kotlin.Any = apiInstance.nexusProcessSpeechToText(audio, storeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling STTAPIApi#nexusProcessSpeechToText")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling STTAPIApi#nexusProcessSpeechToText")
    e.printStackTrace()
}
```

### Parameters
| **audio** | **java.io.File**| The audio file to convert to text | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **storeId** | **kotlin.String**| The store ID | |

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

