# AgentsOpenResponsesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetAgentsV1ResponsesByid**](AgentsOpenResponsesApi.md#chatGetAgentsV1ResponsesByid) | **GET** /v1/chat/agents/v1/responses/{id} | Get a stored response |
| [**chatGetAgentsV1ResponsesModels**](AgentsOpenResponsesApi.md#chatGetAgentsV1ResponsesModels) | **GET** /v1/chat/agents/v1/responses/models | List agents as models |
| [**chatPostAgentsV1Responses**](AgentsOpenResponsesApi.md#chatPostAgentsV1Responses) | **POST** /v1/chat/agents/v1/responses | Create a response |


<a id="chatGetAgentsV1ResponsesByid"></a>
# **chatGetAgentsV1ResponsesByid**
> ChatResponseObject chatGetAgentsV1ResponsesByid(id)

Get a stored response

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenResponsesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ChatResponseObject = apiInstance.chatGetAgentsV1ResponsesByid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenResponsesApi#chatGetAgentsV1ResponsesByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenResponsesApi#chatGetAgentsV1ResponsesByid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ChatResponseObject**](ChatResponseObject.md)

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

<a id="chatGetAgentsV1ResponsesModels"></a>
# **chatGetAgentsV1ResponsesModels**
> kotlin.Any chatGetAgentsV1ResponsesModels()

List agents as models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenResponsesApi()
try {
    val result : kotlin.Any = apiInstance.chatGetAgentsV1ResponsesModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenResponsesApi#chatGetAgentsV1ResponsesModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenResponsesApi#chatGetAgentsV1ResponsesModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="chatPostAgentsV1Responses"></a>
# **chatPostAgentsV1Responses**
> ChatResponseObject chatPostAgentsV1Responses(chatPostAgentsV1ResponsesRequest)

Create a response

Open Responses API for creating agent responses.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsOpenResponsesApi()
val chatPostAgentsV1ResponsesRequest : ChatPostAgentsV1ResponsesRequest =  // ChatPostAgentsV1ResponsesRequest | 
try {
    val result : ChatResponseObject = apiInstance.chatPostAgentsV1Responses(chatPostAgentsV1ResponsesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsOpenResponsesApi#chatPostAgentsV1Responses")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsOpenResponsesApi#chatPostAgentsV1Responses")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsV1ResponsesRequest** | [**ChatPostAgentsV1ResponsesRequest**](ChatPostAgentsV1ResponsesRequest.md)|  | |

### Return type

[**ChatResponseObject**](ChatResponseObject.md)

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

