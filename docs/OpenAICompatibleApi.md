# OpenAICompatibleApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aiCreateChatCompletion**](OpenAICompatibleApi.md#aiCreateChatCompletion) | **POST** /v1/chat/completions | Create chat completion |
| [**aiCreateCompletion**](OpenAICompatibleApi.md#aiCreateCompletion) | **POST** /v1/completions | Create completion (legacy text) |
| [**aiCreateEmbeddings**](OpenAICompatibleApi.md#aiCreateEmbeddings) | **POST** /v1/embeddings | Create embeddings |
| [**aiCreateImage**](OpenAICompatibleApi.md#aiCreateImage) | **POST** /v1/images/generations | Create image |
| [**aiCreateSpeech**](OpenAICompatibleApi.md#aiCreateSpeech) | **POST** /v1/audio/speech | Create speech (text-to-speech) |
| [**aiCreateTranscription**](OpenAICompatibleApi.md#aiCreateTranscription) | **POST** /v1/audio/transcriptions | Create transcription (speech-to-text) |
| [**aiRerank**](OpenAICompatibleApi.md#aiRerank) | **POST** /v1/rerank | Rerank documents against a query |


<a id="aiCreateChatCompletion"></a>
# **aiCreateChatCompletion**
> AiChatCompletionResponse aiCreateChatCompletion(aiChatCompletionRequest)

Create chat completion

OpenAI-compatible chat completions. Set &#x60;stream: true&#x60; for an SSE token stream (&#x60;text/event-stream&#x60;), otherwise a single JSON response. &#x60;model&#x60; accepts any model id from &#x60;GET /v1/models&#x60; (including the Zen ladder). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiChatCompletionRequest : AiChatCompletionRequest =  // AiChatCompletionRequest | 
try {
    val result : AiChatCompletionResponse = apiInstance.aiCreateChatCompletion(aiChatCompletionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateChatCompletion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateChatCompletion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiChatCompletionRequest** | [**AiChatCompletionRequest**](AiChatCompletionRequest.md)|  | |

### Return type

[**AiChatCompletionResponse**](AiChatCompletionResponse.md)

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

<a id="aiCreateCompletion"></a>
# **aiCreateCompletion**
> kotlin.Any aiCreateCompletion(aiCompletionRequest)

Create completion (legacy text)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiCompletionRequest : AiCompletionRequest =  // AiCompletionRequest | 
try {
    val result : kotlin.Any = apiInstance.aiCreateCompletion(aiCompletionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateCompletion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateCompletion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiCompletionRequest** | [**AiCompletionRequest**](AiCompletionRequest.md)|  | |

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

<a id="aiCreateEmbeddings"></a>
# **aiCreateEmbeddings**
> AiEmbeddingResponse aiCreateEmbeddings(aiEmbeddingRequest)

Create embeddings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiEmbeddingRequest : AiEmbeddingRequest =  // AiEmbeddingRequest | 
try {
    val result : AiEmbeddingResponse = apiInstance.aiCreateEmbeddings(aiEmbeddingRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateEmbeddings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateEmbeddings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiEmbeddingRequest** | [**AiEmbeddingRequest**](AiEmbeddingRequest.md)|  | |

### Return type

[**AiEmbeddingResponse**](AiEmbeddingResponse.md)

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

<a id="aiCreateImage"></a>
# **aiCreateImage**
> AiImageResponse aiCreateImage(aiImageGenerationRequest)

Create image

OpenAI-compatible text-to-image generation.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiImageGenerationRequest : AiImageGenerationRequest =  // AiImageGenerationRequest | 
try {
    val result : AiImageResponse = apiInstance.aiCreateImage(aiImageGenerationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiImageGenerationRequest** | [**AiImageGenerationRequest**](AiImageGenerationRequest.md)|  | |

### Return type

[**AiImageResponse**](AiImageResponse.md)

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

<a id="aiCreateSpeech"></a>
# **aiCreateSpeech**
> java.io.File aiCreateSpeech(aiSpeechRequest)

Create speech (text-to-speech)

OpenAI-compatible text-to-speech. Returns binary audio.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiSpeechRequest : AiSpeechRequest =  // AiSpeechRequest | 
try {
    val result : java.io.File = apiInstance.aiCreateSpeech(aiSpeechRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateSpeech")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateSpeech")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiSpeechRequest** | [**AiSpeechRequest**](AiSpeechRequest.md)|  | |

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
 - **Accept**: application/octet-stream, application/json

<a id="aiCreateTranscription"></a>
# **aiCreateTranscription**
> AiTranscriptionResponse aiCreateTranscription(file, model, language, prompt, responseFormat, temperature)

Create transcription (speech-to-text)

OpenAI-compatible speech-to-text (Whisper interface).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val model : kotlin.String = model_example // kotlin.String | 
val language : kotlin.String = language_example // kotlin.String | 
val prompt : kotlin.String = prompt_example // kotlin.String | 
val responseFormat : kotlin.String = responseFormat_example // kotlin.String | 
val temperature : java.math.BigDecimal = 8.14 // java.math.BigDecimal | 
try {
    val result : AiTranscriptionResponse = apiInstance.aiCreateTranscription(file, model, language, prompt, responseFormat, temperature)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiCreateTranscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiCreateTranscription")
    e.printStackTrace()
}
```

### Parameters
| **file** | **java.io.File**|  | |
| **model** | **kotlin.String**|  | |
| **language** | **kotlin.String**|  | [optional] |
| **prompt** | **kotlin.String**|  | [optional] |
| **responseFormat** | **kotlin.String**|  | [optional] [enum: json, text, srt, verbose_json, vtt] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **temperature** | **java.math.BigDecimal**|  | [optional] |

### Return type

[**AiTranscriptionResponse**](AiTranscriptionResponse.md)

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

<a id="aiRerank"></a>
# **aiRerank**
> kotlin.Any aiRerank(aiRerankRequest)

Rerank documents against a query

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpenAICompatibleApi()
val aiRerankRequest : AiRerankRequest =  // AiRerankRequest | 
try {
    val result : kotlin.Any = apiInstance.aiRerank(aiRerankRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpenAICompatibleApi#aiRerank")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpenAICompatibleApi#aiRerank")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiRerankRequest** | [**AiRerankRequest**](AiRerankRequest.md)|  | |

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

