# AgentsOpenAICompatibleApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetAgentsV1Models**](AgentsOpenAICompatibleApi.md#chatGetAgentsV1Models) | **GET** /v1/chat/agents/v1/models | List agents as models |
| [**chatGetAgentsV1ModelsBymodel**](AgentsOpenAICompatibleApi.md#chatGetAgentsV1ModelsBymodel) | **GET** /v1/chat/agents/v1/models/{model} | Get agent/model details |
| [**chatPostAgentsV1ChatCompletions**](AgentsOpenAICompatibleApi.md#chatPostAgentsV1ChatCompletions) | **POST** /v1/chat/agents/v1/chat/completions | OpenAI-compatible chat completions |


<a id="chatGetAgentsV1Models"></a>
# **chatGetAgentsV1Models**
> ChatGetAgentsV1Models200Response chatGetAgentsV1Models()

List agents as models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenAICompatibleApi()
try {
    val result : ChatGetAgentsV1Models200Response = apiInstance.chatGetAgentsV1Models()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenAICompatibleApi#chatGetAgentsV1Models")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenAICompatibleApi#chatGetAgentsV1Models")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetAgentsV1Models200Response**](ChatGetAgentsV1Models200Response.md)

### Authorization


Configure BearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure BearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatGetAgentsV1ModelsBymodel"></a>
# **chatGetAgentsV1ModelsBymodel**
> ChatModelObject chatGetAgentsV1ModelsBymodel(model)

Get agent/model details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenAICompatibleApi()
val model : kotlin.String = model_example // kotlin.String | 
try {
    val result : ChatModelObject = apiInstance.chatGetAgentsV1ModelsBymodel(model)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenAICompatibleApi#chatGetAgentsV1ModelsBymodel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenAICompatibleApi#chatGetAgentsV1ModelsBymodel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **model** | **kotlin.String**|  | |

### Return type

[**ChatModelObject**](ChatModelObject.md)

### Authorization


Configure BearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure BearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="chatPostAgentsV1ChatCompletions"></a>
# **chatPostAgentsV1ChatCompletions**
> ChatChatCompletion chatPostAgentsV1ChatCompletions(chatPostAgentsV1ChatCompletionsRequest)

OpenAI-compatible chat completions

Send chat messages to an agent using OpenAI format. Requires API key auth.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenAICompatibleApi()
val chatPostAgentsV1ChatCompletionsRequest : ChatPostAgentsV1ChatCompletionsRequest =  // ChatPostAgentsV1ChatCompletionsRequest | 
try {
    val result : ChatChatCompletion = apiInstance.chatPostAgentsV1ChatCompletions(chatPostAgentsV1ChatCompletionsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenAICompatibleApi#chatPostAgentsV1ChatCompletions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenAICompatibleApi#chatPostAgentsV1ChatCompletions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsV1ChatCompletionsRequest** | [**ChatPostAgentsV1ChatCompletionsRequest**](ChatPostAgentsV1ChatCompletionsRequest.md)|  | |

### Return type

[**ChatChatCompletion**](ChatChatCompletion.md)

### Authorization


Configure BearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure BearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

