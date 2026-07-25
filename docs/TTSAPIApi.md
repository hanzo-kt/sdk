# TTSAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGenerateTextToSpeechAudio**](TTSAPIApi.md#cloudApiControllerGenerateTextToSpeechAudio) | **POST** /v1/cloud/generate-text-to-speech-audio | Api Controller Generate Text To Speech Audio |
| [**cloudApiControllerGenerateTextToSpeechAudioStream**](TTSAPIApi.md#cloudApiControllerGenerateTextToSpeechAudioStream) | **GET** /v1/cloud/generate-text-to-speech-audio-stream | Api Controller Generate Text To Speech Audio Stream |
| [**nexusGenerateTextToSpeechAudio**](TTSAPIApi.md#nexusGenerateTextToSpeechAudio) | **POST** /v1/nexus/generate-text-to-speech-audio | generate Text To Speech Audio |
| [**nexusGenerateTextToSpeechAudioStream**](TTSAPIApi.md#nexusGenerateTextToSpeechAudioStream) | **GET** /v1/nexus/generate-text-to-speech-audio-stream | generate Text To Speech Audio Stream |


<a id="cloudApiControllerGenerateTextToSpeechAudio"></a>
# **cloudApiControllerGenerateTextToSpeechAudio**
> kotlin.collections.List&lt;kotlin.ByteArray&gt; cloudApiControllerGenerateTextToSpeechAudio(body)

Api Controller Generate Text To Speech Audio

convert text to speech

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TTSAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The text to convert to speech
try {
    val result : kotlin.collections.List<kotlin.ByteArray> = apiInstance.cloudApiControllerGenerateTextToSpeechAudio(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TTSAPIApi#cloudApiControllerGenerateTextToSpeechAudio")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TTSAPIApi#cloudApiControllerGenerateTextToSpeechAudio")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The text to convert to speech | |

### Return type

**kotlin.collections.List&lt;kotlin.ByteArray&gt;**

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

<a id="cloudApiControllerGenerateTextToSpeechAudioStream"></a>
# **cloudApiControllerGenerateTextToSpeechAudioStream**
> kotlin.Any cloudApiControllerGenerateTextToSpeechAudioStream(storeId, messageId)

Api Controller Generate Text To Speech Audio Stream

convert text to speech with streaming

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TTSAPIApi()
val storeId : kotlin.String = storeId_example // kotlin.String | The store ID
val messageId : kotlin.String = messageId_example // kotlin.String | The message ID
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGenerateTextToSpeechAudioStream(storeId, messageId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TTSAPIApi#cloudApiControllerGenerateTextToSpeechAudioStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TTSAPIApi#cloudApiControllerGenerateTextToSpeechAudioStream")
    e.printStackTrace()
}
```

### Parameters
| **storeId** | **kotlin.String**| The store ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **messageId** | **kotlin.String**| The message ID | |

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

<a id="nexusGenerateTextToSpeechAudio"></a>
# **nexusGenerateTextToSpeechAudio**
> java.io.File nexusGenerateTextToSpeechAudio(body)

generate Text To Speech Audio

Convert text to speech

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TTSAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The text to convert to speech
try {
    val result : java.io.File = apiInstance.nexusGenerateTextToSpeechAudio(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TTSAPIApi#nexusGenerateTextToSpeechAudio")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TTSAPIApi#nexusGenerateTextToSpeechAudio")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The text to convert to speech | |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream

<a id="nexusGenerateTextToSpeechAudioStream"></a>
# **nexusGenerateTextToSpeechAudioStream**
> kotlin.String nexusGenerateTextToSpeechAudioStream(storeId, messageId)

generate Text To Speech Audio Stream

Convert text to speech with streaming

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TTSAPIApi()
val storeId : kotlin.String = storeId_example // kotlin.String | The store ID
val messageId : kotlin.String = messageId_example // kotlin.String | The message ID
try {
    val result : kotlin.String = apiInstance.nexusGenerateTextToSpeechAudioStream(storeId, messageId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TTSAPIApi#nexusGenerateTextToSpeechAudioStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TTSAPIApi#nexusGenerateTextToSpeechAudioStream")
    e.printStackTrace()
}
```

### Parameters
| **storeId** | **kotlin.String**| The store ID | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **messageId** | **kotlin.String**| The message ID | |

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

