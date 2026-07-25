# FilesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteFiles**](FilesApi.md#chatDeleteFiles) | **DELETE** /v1/chat/files | Delete files |
| [**chatGetFiles**](FilesApi.md#chatGetFiles) | **GET** /v1/chat/files | List user files |
| [**chatGetFilesAgentByagentId**](FilesApi.md#chatGetFilesAgentByagentId) | **GET** /v1/chat/files/agent/{agent_id} | Get files for an agent |
| [**chatGetFilesCodeDownloadBysessionIdByfileid**](FilesApi.md#chatGetFilesCodeDownloadBysessionIdByfileid) | **GET** /v1/chat/files/code/download/{session_id}/{fileId} | Download code execution output |
| [**chatGetFilesConfig**](FilesApi.md#chatGetFilesConfig) | **GET** /v1/chat/files/config | Get file upload configuration |
| [**chatGetFilesDownloadByuseridByfileId**](FilesApi.md#chatGetFilesDownloadByuseridByfileId) | **GET** /v1/chat/files/download/{userId}/{file_id} | Download a file |
| [**chatPostFiles**](FilesApi.md#chatPostFiles) | **POST** /v1/chat/files | Upload a file |
| [**execDownloadFile**](FilesApi.md#execDownloadFile) | **GET** /v1/download/{id} | Download a produced file by id |
| [**execListSessionFiles**](FilesApi.md#execListSessionFiles) | **GET** /v1/files/{session_id} | List the files produced in a session |
| [**execUploadFile**](FilesApi.md#execUploadFile) | **POST** /v1/upload | Upload a file into a session |


<a id="chatDeleteFiles"></a>
# **chatDeleteFiles**
> kotlin.Any chatDeleteFiles(chatDeleteFilesRequest)

Delete files

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val chatDeleteFilesRequest : ChatDeleteFilesRequest =  // ChatDeleteFilesRequest | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteFiles(chatDeleteFilesRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatDeleteFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatDeleteFiles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatDeleteFilesRequest** | [**ChatDeleteFilesRequest**](ChatDeleteFilesRequest.md)|  | |

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

<a id="chatGetFiles"></a>
# **chatGetFiles**
> kotlin.collections.List&lt;ChatFile&gt; chatGetFiles()

List user files

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
try {
    val result : kotlin.collections.List<ChatFile> = apiInstance.chatGetFiles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatGetFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatGetFiles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatFile&gt;**](ChatFile.md)

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

<a id="chatGetFilesAgentByagentId"></a>
# **chatGetFilesAgentByagentId**
> kotlin.collections.List&lt;ChatFile&gt; chatGetFilesAgentByagentId(agentId)

Get files for an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val agentId : kotlin.String = agentId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ChatFile> = apiInstance.chatGetFilesAgentByagentId(agentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatGetFilesAgentByagentId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatGetFilesAgentByagentId")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **agentId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;ChatFile&gt;**](ChatFile.md)

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

<a id="chatGetFilesCodeDownloadBysessionIdByfileid"></a>
# **chatGetFilesCodeDownloadBysessionIdByfileid**
> java.io.File chatGetFilesCodeDownloadBysessionIdByfileid(sessionId, fileId)

Download code execution output

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val sessionId : kotlin.String = sessionId_example // kotlin.String | 
val fileId : kotlin.String = fileId_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.chatGetFilesCodeDownloadBysessionIdByfileid(sessionId, fileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatGetFilesCodeDownloadBysessionIdByfileid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatGetFilesCodeDownloadBysessionIdByfileid")
    e.printStackTrace()
}
```

### Parameters
| **sessionId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **fileId** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream

<a id="chatGetFilesConfig"></a>
# **chatGetFilesConfig**
> kotlin.Any chatGetFilesConfig()

Get file upload configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
try {
    val result : kotlin.Any = apiInstance.chatGetFilesConfig()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatGetFilesConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatGetFilesConfig")
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

<a id="chatGetFilesDownloadByuseridByfileId"></a>
# **chatGetFilesDownloadByuseridByfileId**
> java.io.File chatGetFilesDownloadByuseridByfileId(userId, fileId)

Download a file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val userId : kotlin.String = userId_example // kotlin.String | 
val fileId : kotlin.String = fileId_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.chatGetFilesDownloadByuseridByfileId(userId, fileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatGetFilesDownloadByuseridByfileId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatGetFilesDownloadByuseridByfileId")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **fileId** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream

<a id="chatPostFiles"></a>
# **chatPostFiles**
> ChatFile chatPostFiles(file, fileId, endpoint, agentId, toolResource, messageFile)

Upload a file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val fileId : kotlin.String = fileId_example // kotlin.String | 
val endpoint : kotlin.String = endpoint_example // kotlin.String | 
val agentId : kotlin.String = agentId_example // kotlin.String | 
val toolResource : kotlin.String = toolResource_example // kotlin.String | 
val messageFile : kotlin.String = messageFile_example // kotlin.String | 
try {
    val result : ChatFile = apiInstance.chatPostFiles(file, fileId, endpoint, agentId, toolResource, messageFile)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#chatPostFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#chatPostFiles")
    e.printStackTrace()
}
```

### Parameters
| **file** | **java.io.File**|  | |
| **fileId** | **kotlin.String**|  | [optional] |
| **endpoint** | **kotlin.String**|  | [optional] |
| **agentId** | **kotlin.String**|  | [optional] |
| **toolResource** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **messageFile** | **kotlin.String**|  | [optional] |

### Return type

[**ChatFile**](ChatFile.md)

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

<a id="execDownloadFile"></a>
# **execDownloadFile**
> java.io.File execDownloadFile(id)

Download a produced file by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.execDownloadFile(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#execDownloadFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#execDownloadFile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/json

<a id="execListSessionFiles"></a>
# **execListSessionFiles**
> ExecListSessionFiles200Response execListSessionFiles(sessionId)

List the files produced in a session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val sessionId : kotlin.String = sessionId_example // kotlin.String | 
try {
    val result : ExecListSessionFiles200Response = apiInstance.execListSessionFiles(sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#execListSessionFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#execListSessionFiles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **kotlin.String**|  | |

### Return type

[**ExecListSessionFiles200Response**](ExecListSessionFiles200Response.md)

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

<a id="execUploadFile"></a>
# **execUploadFile**
> ExecUploadFile200Response execUploadFile(file, sessionId)

Upload a file into a session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FilesApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | 
val sessionId : kotlin.String = sessionId_example // kotlin.String | 
try {
    val result : ExecUploadFile200Response = apiInstance.execUploadFile(file, sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FilesApi#execUploadFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FilesApi#execUploadFile")
    e.printStackTrace()
}
```

### Parameters
| **file** | **java.io.File**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **kotlin.String**|  | [optional] |

### Return type

[**ExecUploadFile200Response**](ExecUploadFile200Response.md)

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

