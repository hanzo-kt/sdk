# SpeechApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetFilesSpeechConfigGet**](SpeechApi.md#chatGetFilesSpeechConfigGet) | **GET** /v1/chat/files/speech/config/get | Get custom speech configuration |
| [**chatGetFilesSpeechTtsVoices**](SpeechApi.md#chatGetFilesSpeechTtsVoices) | **GET** /v1/chat/files/speech/tts/voices | Get available TTS voices |
| [**chatPostFilesSpeechStt**](SpeechApi.md#chatPostFilesSpeechStt) | **POST** /v1/chat/files/speech/stt | Speech to text |
| [**chatPostFilesSpeechTts**](SpeechApi.md#chatPostFilesSpeechTts) | **POST** /v1/chat/files/speech/tts | Stream text to speech |
| [**chatPostFilesSpeechTtsManual**](SpeechApi.md#chatPostFilesSpeechTtsManual) | **POST** /v1/chat/files/speech/tts/manual | Manual text to speech |


<a id="chatGetFilesSpeechConfigGet"></a>
# **chatGetFilesSpeechConfigGet**
> kotlin.Any chatGetFilesSpeechConfigGet()

Get custom speech configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpeechApi()
try {
    val result : kotlin.Any = apiInstance.chatGetFilesSpeechConfigGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpeechApi#chatGetFilesSpeechConfigGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpeechApi#chatGetFilesSpeechConfigGet")
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

<a id="chatGetFilesSpeechTtsVoices"></a>
# **chatGetFilesSpeechTtsVoices**
> kotlin.Any chatGetFilesSpeechTtsVoices()

Get available TTS voices

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpeechApi()
try {
    val result : kotlin.Any = apiInstance.chatGetFilesSpeechTtsVoices()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpeechApi#chatGetFilesSpeechTtsVoices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpeechApi#chatGetFilesSpeechTtsVoices")
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

<a id="chatPostFilesSpeechStt"></a>
# **chatPostFilesSpeechStt**
> kotlin.Any chatPostFilesSpeechStt(audio)

Speech to text

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpeechApi()
val audio : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : kotlin.Any = apiInstance.chatPostFilesSpeechStt(audio)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpeechApi#chatPostFilesSpeechStt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpeechApi#chatPostFilesSpeechStt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **audio** | **java.io.File**|  | |

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

<a id="chatPostFilesSpeechTts"></a>
# **chatPostFilesSpeechTts**
> java.io.File chatPostFilesSpeechTts(chatPostFilesSpeechTtsRequest)

Stream text to speech

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpeechApi()
val chatPostFilesSpeechTtsRequest : ChatPostFilesSpeechTtsRequest =  // ChatPostFilesSpeechTtsRequest | 
try {
    val result : java.io.File = apiInstance.chatPostFilesSpeechTts(chatPostFilesSpeechTtsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpeechApi#chatPostFilesSpeechTts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpeechApi#chatPostFilesSpeechTts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostFilesSpeechTtsRequest** | [**ChatPostFilesSpeechTtsRequest**](ChatPostFilesSpeechTtsRequest.md)|  | |

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
 - **Accept**: Not defined

<a id="chatPostFilesSpeechTtsManual"></a>
# **chatPostFilesSpeechTtsManual**
> kotlin.Any chatPostFilesSpeechTtsManual(text, voice)

Manual text to speech

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SpeechApi()
val text : kotlin.String = text_example // kotlin.String | 
val voice : kotlin.String = voice_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostFilesSpeechTtsManual(text, voice)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SpeechApi#chatPostFilesSpeechTtsManual")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SpeechApi#chatPostFilesSpeechTtsManual")
    e.printStackTrace()
}
```

### Parameters
| **text** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voice** | **kotlin.String**|  | [optional] |

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

