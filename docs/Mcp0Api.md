# McpApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetMcpServer**](McpApi.md#autoGetMcpServer) | **GET** /v1/auto/projects/{projectId}/mcp-server | Get MCP server configuration for a project |
| [**flowGetMcpServer**](McpApi.md#flowGetMcpServer) | **GET** /v1/flow/projects/{projectId}/mcp-server | Get MCP server configuration for a project |


<a id="autoGetMcpServer"></a>
# **autoGetMcpServer**
> kotlin.Any autoGetMcpServer(projectId)

Get MCP server configuration for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = McpApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetMcpServer(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling McpApi#autoGetMcpServer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling McpApi#autoGetMcpServer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

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

<a id="flowGetMcpServer"></a>
# **flowGetMcpServer**
> kotlin.Any flowGetMcpServer(projectId)

Get MCP server configuration for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = McpApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetMcpServer(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling McpApi#flowGetMcpServer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling McpApi#flowGetMcpServer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

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

