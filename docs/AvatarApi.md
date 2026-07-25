# AvatarApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatPostAssistantsV2AvatarByassistantId**](AvatarApi.md#chatPostAssistantsV2AvatarByassistantId) | **POST** /v1/chat/assistants/v2/avatar/{assistant_id} | Upload assistant avatar (v2) |
| [**chatPostFilesImagesAgentsByagentIdAvatar**](AvatarApi.md#chatPostFilesImagesAgentsByagentIdAvatar) | **POST** /v1/chat/files/images/agents/{agent_id}/avatar | Upload agent avatar |
| [**chatPostFilesImagesAssistantsByassistantIdAvatar**](AvatarApi.md#chatPostFilesImagesAssistantsByassistantIdAvatar) | **POST** /v1/chat/files/images/assistants/{assistant_id}/avatar | Upload assistant avatar (v1) |
| [**chatPostFilesImagesAvatar**](AvatarApi.md#chatPostFilesImagesAvatar) | **POST** /v1/chat/files/images/avatar | Upload user avatar |


<a id="chatPostAssistantsV2AvatarByassistantId"></a>
# **chatPostAssistantsV2AvatarByassistantId**
> kotlin.Any chatPostAssistantsV2AvatarByassistantId(assistantId, file, metadata)

Upload assistant avatar (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AvatarApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val metadata : kotlin.String = metadata_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV2AvatarByassistantId(assistantId, file, metadata)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AvatarApi#chatPostAssistantsV2AvatarByassistantId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AvatarApi#chatPostAssistantsV2AvatarByassistantId")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
| **file** | **java.io.File**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **metadata** | **kotlin.String**|  | [optional] |

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

<a id="chatPostFilesImagesAgentsByagentIdAvatar"></a>
# **chatPostFilesImagesAgentsByagentIdAvatar**
> kotlin.Any chatPostFilesImagesAgentsByagentIdAvatar(agentId, file, metadata)

Upload agent avatar

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AvatarApi()
val agentId : kotlin.String = agentId_example // kotlin.String | 
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val metadata : kotlin.String = metadata_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostFilesImagesAgentsByagentIdAvatar(agentId, file, metadata)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AvatarApi#chatPostFilesImagesAgentsByagentIdAvatar")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AvatarApi#chatPostFilesImagesAgentsByagentIdAvatar")
    e.printStackTrace()
}
```

### Parameters
| **agentId** | **kotlin.String**|  | |
| **file** | **java.io.File**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **metadata** | **kotlin.String**|  | [optional] |

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

<a id="chatPostFilesImagesAssistantsByassistantIdAvatar"></a>
# **chatPostFilesImagesAssistantsByassistantIdAvatar**
> kotlin.Any chatPostFilesImagesAssistantsByassistantIdAvatar(assistantId, file, metadata)

Upload assistant avatar (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AvatarApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val metadata : kotlin.String = metadata_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostFilesImagesAssistantsByassistantIdAvatar(assistantId, file, metadata)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AvatarApi#chatPostFilesImagesAssistantsByassistantIdAvatar")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AvatarApi#chatPostFilesImagesAssistantsByassistantIdAvatar")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
| **file** | **java.io.File**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **metadata** | **kotlin.String**|  | [optional] |

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

<a id="chatPostFilesImagesAvatar"></a>
# **chatPostFilesImagesAvatar**
> ChatPostFilesImagesAvatar200Response chatPostFilesImagesAvatar(file, manual)

Upload user avatar

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AvatarApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val manual : kotlin.String = manual_example // kotlin.String | 
try {
    val result : ChatPostFilesImagesAvatar200Response = apiInstance.chatPostFilesImagesAvatar(file, manual)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AvatarApi#chatPostFilesImagesAvatar")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AvatarApi#chatPostFilesImagesAvatar")
    e.printStackTrace()
}
```

### Parameters
| **file** | **java.io.File**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **manual** | **kotlin.String**|  | [optional] |

### Return type

[**ChatPostFilesImagesAvatar200Response**](ChatPostFilesImagesAvatar200Response.md)

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

