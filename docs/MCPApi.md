# MCPApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**automationsMcp**](MCPApi.md#automationsMcp) | **POST** /v1/automations/mcp | JSON-RPC 2.0 tool surface over connector actions |
| [**chatDeleteMcpServersByservername**](MCPApi.md#chatDeleteMcpServersByservername) | **DELETE** /v1/chat/mcp/servers/{serverName} | Delete an MCP server |
| [**chatGetMcpByservernameAuthValues**](MCPApi.md#chatGetMcpByservernameAuthValues) | **GET** /v1/chat/mcp/{serverName}/auth-values | Check which auth values exist for an MCP server |
| [**chatGetMcpByservernameOauthCallback**](MCPApi.md#chatGetMcpByservernameOauthCallback) | **GET** /v1/chat/mcp/{serverName}/oauth/callback | MCP OAuth callback |
| [**chatGetMcpByservernameOauthInitiate**](MCPApi.md#chatGetMcpByservernameOauthInitiate) | **GET** /v1/chat/mcp/{serverName}/oauth/initiate | Initiate MCP OAuth flow |
| [**chatGetMcpConnectionStatus**](MCPApi.md#chatGetMcpConnectionStatus) | **GET** /v1/chat/mcp/connection/status | Get connection status for all MCP servers |
| [**chatGetMcpConnectionStatusByservername**](MCPApi.md#chatGetMcpConnectionStatusByservername) | **GET** /v1/chat/mcp/connection/status/{serverName} | Get connection status for a specific MCP server |
| [**chatGetMcpOauthStatusByflowid**](MCPApi.md#chatGetMcpOauthStatusByflowid) | **GET** /v1/chat/mcp/oauth/status/{flowId} | Check OAuth flow status |
| [**chatGetMcpOauthTokensByflowid**](MCPApi.md#chatGetMcpOauthTokensByflowid) | **GET** /v1/chat/mcp/oauth/tokens/{flowId} | Get OAuth tokens for a completed flow |
| [**chatGetMcpServers**](MCPApi.md#chatGetMcpServers) | **GET** /v1/chat/mcp/servers | List user-managed MCP servers |
| [**chatGetMcpServersByservername**](MCPApi.md#chatGetMcpServersByservername) | **GET** /v1/chat/mcp/servers/{serverName} | Get an MCP server by name |
| [**chatGetMcpTools**](MCPApi.md#chatGetMcpTools) | **GET** /v1/chat/mcp/tools | Get all available MCP tools |
| [**chatPatchMcpServersByservername**](MCPApi.md#chatPatchMcpServersByservername) | **PATCH** /v1/chat/mcp/servers/{serverName} | Update an MCP server |
| [**chatPostMcpByservernameOauthBind**](MCPApi.md#chatPostMcpByservernameOauthBind) | **POST** /v1/chat/mcp/{serverName}/oauth/bind | Set CSRF binding cookie for MCP OAuth |
| [**chatPostMcpByservernameReinitialize**](MCPApi.md#chatPostMcpByservernameReinitialize) | **POST** /v1/chat/mcp/{serverName}/reinitialize | Reinitialize an MCP server |
| [**chatPostMcpOauthCancelByservername**](MCPApi.md#chatPostMcpOauthCancelByservername) | **POST** /v1/chat/mcp/oauth/cancel/{serverName} | Cancel an OAuth flow |
| [**chatPostMcpServers**](MCPApi.md#chatPostMcpServers) | **POST** /v1/chat/mcp/servers | Create a user-managed MCP server |


<a id="automationsMcp"></a>
# **automationsMcp**
> AutomationsMcpResponse automationsMcp(automationsMcpRequest)

JSON-RPC 2.0 tool surface over connector actions

HIP-0300 JSON-RPC 2.0. Methods: &#x60;initialize&#x60;, &#x60;ping&#x60;, &#x60;tools/list&#x60;, &#x60;tools/call&#x60;. Every connector action is a tool named &#x60;&lt;connector&gt;_&lt;action&gt;&#x60;. JSON-RPC errors are returned with HTTP 200 and an &#x60;error&#x60; member. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val automationsMcpRequest : AutomationsMcpRequest =  // AutomationsMcpRequest | 
try {
    val result : AutomationsMcpResponse = apiInstance.automationsMcp(automationsMcpRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#automationsMcp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#automationsMcp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **automationsMcpRequest** | [**AutomationsMcpRequest**](AutomationsMcpRequest.md)|  | |

### Return type

[**AutomationsMcpResponse**](AutomationsMcpResponse.md)

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

<a id="chatDeleteMcpServersByservername"></a>
# **chatDeleteMcpServersByservername**
> kotlin.Any chatDeleteMcpServersByservername(serverName)

Delete an MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteMcpServersByservername(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatDeleteMcpServersByservername")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatDeleteMcpServersByservername")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

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

<a id="chatGetMcpByservernameAuthValues"></a>
# **chatGetMcpByservernameAuthValues**
> ChatGetMcpByservernameAuthValues200Response chatGetMcpByservernameAuthValues(serverName)

Check which auth values exist for an MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : ChatGetMcpByservernameAuthValues200Response = apiInstance.chatGetMcpByservernameAuthValues(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpByservernameAuthValues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpByservernameAuthValues")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

### Return type

[**ChatGetMcpByservernameAuthValues200Response**](ChatGetMcpByservernameAuthValues200Response.md)

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

<a id="chatGetMcpByservernameOauthCallback"></a>
# **chatGetMcpByservernameOauthCallback**
> chatGetMcpByservernameOauthCallback(serverName, code, state)

MCP OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
val code : kotlin.String = code_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
try {
    apiInstance.chatGetMcpByservernameOauthCallback(serverName, code, state)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpByservernameOauthCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpByservernameOauthCallback")
    e.printStackTrace()
}
```

### Parameters
| **serverName** | **kotlin.String**|  | |
| **code** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="chatGetMcpByservernameOauthInitiate"></a>
# **chatGetMcpByservernameOauthInitiate**
> chatGetMcpByservernameOauthInitiate(serverName, userId, flowId)

Initiate MCP OAuth flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
val userId : kotlin.String = userId_example // kotlin.String | 
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    apiInstance.chatGetMcpByservernameOauthInitiate(serverName, userId, flowId)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpByservernameOauthInitiate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpByservernameOauthInitiate")
    e.printStackTrace()
}
```

### Parameters
| **serverName** | **kotlin.String**|  | |
| **userId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="chatGetMcpConnectionStatus"></a>
# **chatGetMcpConnectionStatus**
> ChatGetMcpConnectionStatus200Response chatGetMcpConnectionStatus()

Get connection status for all MCP servers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
try {
    val result : ChatGetMcpConnectionStatus200Response = apiInstance.chatGetMcpConnectionStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpConnectionStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpConnectionStatus")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetMcpConnectionStatus200Response**](ChatGetMcpConnectionStatus200Response.md)

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

<a id="chatGetMcpConnectionStatusByservername"></a>
# **chatGetMcpConnectionStatusByservername**
> kotlin.Any chatGetMcpConnectionStatusByservername(serverName)

Get connection status for a specific MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetMcpConnectionStatusByservername(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpConnectionStatusByservername")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpConnectionStatusByservername")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

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

<a id="chatGetMcpOauthStatusByflowid"></a>
# **chatGetMcpOauthStatusByflowid**
> ChatGetMcpOauthStatusByflowid200Response chatGetMcpOauthStatusByflowid(flowId)

Check OAuth flow status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : ChatGetMcpOauthStatusByflowid200Response = apiInstance.chatGetMcpOauthStatusByflowid(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpOauthStatusByflowid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpOauthStatusByflowid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

### Return type

[**ChatGetMcpOauthStatusByflowid200Response**](ChatGetMcpOauthStatusByflowid200Response.md)

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

<a id="chatGetMcpOauthTokensByflowid"></a>
# **chatGetMcpOauthTokensByflowid**
> kotlin.Any chatGetMcpOauthTokensByflowid(flowId)

Get OAuth tokens for a completed flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetMcpOauthTokensByflowid(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpOauthTokensByflowid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpOauthTokensByflowid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

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

<a id="chatGetMcpServers"></a>
# **chatGetMcpServers**
> kotlin.Any chatGetMcpServers(limit, after, search)

List user-managed MCP servers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
val after : kotlin.String = after_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetMcpServers(limit, after, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpServers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpServers")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**|  | [optional] |
| **after** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

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

<a id="chatGetMcpServersByservername"></a>
# **chatGetMcpServersByservername**
> kotlin.Any chatGetMcpServersByservername(serverName)

Get an MCP server by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetMcpServersByservername(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpServersByservername")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpServersByservername")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

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

<a id="chatGetMcpTools"></a>
# **chatGetMcpTools**
> kotlin.Any chatGetMcpTools()

Get all available MCP tools

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
try {
    val result : kotlin.Any = apiInstance.chatGetMcpTools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatGetMcpTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatGetMcpTools")
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

<a id="chatPatchMcpServersByservername"></a>
# **chatPatchMcpServersByservername**
> kotlin.Any chatPatchMcpServersByservername(serverName, body)

Update an MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPatchMcpServersByservername(serverName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatPatchMcpServersByservername")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatPatchMcpServersByservername")
    e.printStackTrace()
}
```

### Parameters
| **serverName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="chatPostMcpByservernameOauthBind"></a>
# **chatPostMcpByservernameOauthBind**
> kotlin.Any chatPostMcpByservernameOauthBind(serverName)

Set CSRF binding cookie for MCP OAuth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostMcpByservernameOauthBind(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatPostMcpByservernameOauthBind")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatPostMcpByservernameOauthBind")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

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

<a id="chatPostMcpByservernameReinitialize"></a>
# **chatPostMcpByservernameReinitialize**
> ChatPostMcpByservernameReinitialize200Response chatPostMcpByservernameReinitialize(serverName)

Reinitialize an MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : ChatPostMcpByservernameReinitialize200Response = apiInstance.chatPostMcpByservernameReinitialize(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatPostMcpByservernameReinitialize")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatPostMcpByservernameReinitialize")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

### Return type

[**ChatPostMcpByservernameReinitialize200Response**](ChatPostMcpByservernameReinitialize200Response.md)

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

<a id="chatPostMcpOauthCancelByservername"></a>
# **chatPostMcpOauthCancelByservername**
> kotlin.Any chatPostMcpOauthCancelByservername(serverName)

Cancel an OAuth flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val serverName : kotlin.String = serverName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostMcpOauthCancelByservername(serverName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatPostMcpOauthCancelByservername")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatPostMcpOauthCancelByservername")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serverName** | **kotlin.String**|  | |

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

<a id="chatPostMcpServers"></a>
# **chatPostMcpServers**
> kotlin.Any chatPostMcpServers(body)

Create a user-managed MCP server

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MCPApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostMcpServers(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MCPApi#chatPostMcpServers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MCPApi#chatPostMcpServers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

