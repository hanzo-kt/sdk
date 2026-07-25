# AgentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteAgentsByid**](AgentsApi.md#chatDeleteAgentsByid) | **DELETE** /v1/chat/agents/{id} | Delete an agent |
| [**chatGetAgents**](AgentsApi.md#chatGetAgents) | **GET** /v1/chat/agents | List agents |
| [**chatGetAgentsByid**](AgentsApi.md#chatGetAgentsByid) | **GET** /v1/chat/agents/{id} | Get an agent (basic info) |
| [**chatGetAgentsByidExpanded**](AgentsApi.md#chatGetAgentsByidExpanded) | **GET** /v1/chat/agents/{id}/expanded | Get agent with full configuration details |
| [**chatGetAgentsCategories**](AgentsApi.md#chatGetAgentsCategories) | **GET** /v1/chat/agents/categories | Get agent categories with counts |
| [**chatGetAgentsChatActive**](AgentsApi.md#chatGetAgentsChatActive) | **GET** /v1/chat/agents/chat/active | Get active generation job IDs |
| [**chatGetAgentsChatStatusByconversationid**](AgentsApi.md#chatGetAgentsChatStatusByconversationid) | **GET** /v1/chat/agents/chat/status/{conversationId} | Check generation status for a conversation |
| [**chatGetAgentsChatStreamBystreamid**](AgentsApi.md#chatGetAgentsChatStreamBystreamid) | **GET** /v1/chat/agents/chat/stream/{streamId} | Subscribe to a generation stream |
| [**chatGetAgentsTools**](AgentsApi.md#chatGetAgentsTools) | **GET** /v1/chat/agents/tools | List available agent tools |
| [**chatGetAgentsToolsBytoolidAuth**](AgentsApi.md#chatGetAgentsToolsBytoolidAuth) | **GET** /v1/chat/agents/tools/{toolId}/auth | Verify tool authentication |
| [**chatGetAgentsToolsCalls**](AgentsApi.md#chatGetAgentsToolsCalls) | **GET** /v1/chat/agents/tools/calls | Get tool call history |
| [**chatPatchAgentsByid**](AgentsApi.md#chatPatchAgentsByid) | **PATCH** /v1/chat/agents/{id} | Update an agent |
| [**chatPostAgents**](AgentsApi.md#chatPostAgents) | **POST** /v1/chat/agents | Create an agent |
| [**chatPostAgentsByidDuplicate**](AgentsApi.md#chatPostAgentsByidDuplicate) | **POST** /v1/chat/agents/{id}/duplicate | Duplicate an agent |
| [**chatPostAgentsByidRevert**](AgentsApi.md#chatPostAgentsByidRevert) | **POST** /v1/chat/agents/{id}/revert | Revert agent to a previous version |
| [**chatPostAgentsChat**](AgentsApi.md#chatPostAgentsChat) | **POST** /v1/chat/agents/chat | Chat with an agent |
| [**chatPostAgentsChatAbort**](AgentsApi.md#chatPostAgentsChatAbort) | **POST** /v1/chat/agents/chat/abort | Abort an ongoing agent generation |
| [**chatPostAgentsChatByendpoint**](AgentsApi.md#chatPostAgentsChatByendpoint) | **POST** /v1/chat/agents/chat/{endpoint} | Chat with an ephemeral agent |
| [**chatPostAgentsToolsBytoolidCall**](AgentsApi.md#chatPostAgentsToolsBytoolidCall) | **POST** /v1/chat/agents/tools/{toolId}/call | Execute a tool call |


<a id="chatDeleteAgentsByid"></a>
# **chatDeleteAgentsByid**
> kotlin.Any chatDeleteAgentsByid(id)

Delete an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAgentsByid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatDeleteAgentsByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatDeleteAgentsByid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="chatGetAgents"></a>
# **chatGetAgents**
> ChatAgentListResponse chatGetAgents(limit, after, sortBy, sortDirection)

List agents

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
val after : kotlin.String = after_example // kotlin.String | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val sortDirection : kotlin.String = sortDirection_example // kotlin.String | 
try {
    val result : ChatAgentListResponse = apiInstance.chatGetAgents(limit, after, sortBy, sortDirection)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgents")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**|  | [optional] |
| **after** | **kotlin.String**|  | [optional] |
| **sortBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sortDirection** | **kotlin.String**|  | [optional] |

### Return type

[**ChatAgentListResponse**](ChatAgentListResponse.md)

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

<a id="chatGetAgentsByid"></a>
# **chatGetAgentsByid**
> ChatAgent chatGetAgentsByid(id)

Get an agent (basic info)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ChatAgent = apiInstance.chatGetAgentsByid(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsByid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ChatAgent**](ChatAgent.md)

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

<a id="chatGetAgentsByidExpanded"></a>
# **chatGetAgentsByidExpanded**
> ChatAgent chatGetAgentsByidExpanded(id)

Get agent with full configuration details

Returns complete agent data including sensitive config (EDIT permission required).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ChatAgent = apiInstance.chatGetAgentsByidExpanded(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsByidExpanded")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsByidExpanded")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ChatAgent**](ChatAgent.md)

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

<a id="chatGetAgentsCategories"></a>
# **chatGetAgentsCategories**
> kotlin.Any chatGetAgentsCategories()

Get agent categories with counts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
try {
    val result : kotlin.Any = apiInstance.chatGetAgentsCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsCategories")
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

<a id="chatGetAgentsChatActive"></a>
# **chatGetAgentsChatActive**
> ChatGetAgentsChatActive200Response chatGetAgentsChatActive()

Get active generation job IDs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
try {
    val result : ChatGetAgentsChatActive200Response = apiInstance.chatGetAgentsChatActive()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsChatActive")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsChatActive")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatGetAgentsChatActive200Response**](ChatGetAgentsChatActive200Response.md)

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

<a id="chatGetAgentsChatStatusByconversationid"></a>
# **chatGetAgentsChatStatusByconversationid**
> ChatGetAgentsChatStatusByconversationid200Response chatGetAgentsChatStatusByconversationid(conversationId)

Check generation status for a conversation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val conversationId : kotlin.String = conversationId_example // kotlin.String | 
try {
    val result : ChatGetAgentsChatStatusByconversationid200Response = apiInstance.chatGetAgentsChatStatusByconversationid(conversationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsChatStatusByconversationid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsChatStatusByconversationid")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conversationId** | **kotlin.String**|  | |

### Return type

[**ChatGetAgentsChatStatusByconversationid200Response**](ChatGetAgentsChatStatusByconversationid200Response.md)

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

<a id="chatGetAgentsChatStreamBystreamid"></a>
# **chatGetAgentsChatStreamBystreamid**
> kotlin.String chatGetAgentsChatStreamBystreamid(streamId, resume)

Subscribe to a generation stream

SSE endpoint for live or replay streaming of agent output.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val streamId : kotlin.String = streamId_example // kotlin.String | 
val resume : kotlin.String = resume_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.chatGetAgentsChatStreamBystreamid(streamId, resume)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsChatStreamBystreamid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsChatStreamBystreamid")
    e.printStackTrace()
}
```

### Parameters
| **streamId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resume** | **kotlin.String**|  | [optional] [enum: true] |

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

<a id="chatGetAgentsTools"></a>
# **chatGetAgentsTools**
> kotlin.collections.List&lt;ChatTool&gt; chatGetAgentsTools()

List available agent tools

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
try {
    val result : kotlin.collections.List<ChatTool> = apiInstance.chatGetAgentsTools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsTools")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatTool&gt;**](ChatTool.md)

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

<a id="chatGetAgentsToolsBytoolidAuth"></a>
# **chatGetAgentsToolsBytoolidAuth**
> ChatGetAgentsToolsBytoolidAuth200Response chatGetAgentsToolsBytoolidAuth(toolId)

Verify tool authentication

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val toolId : kotlin.String = toolId_example // kotlin.String | 
try {
    val result : ChatGetAgentsToolsBytoolidAuth200Response = apiInstance.chatGetAgentsToolsBytoolidAuth(toolId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsToolsBytoolidAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsToolsBytoolidAuth")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **toolId** | **kotlin.String**|  | |

### Return type

[**ChatGetAgentsToolsBytoolidAuth200Response**](ChatGetAgentsToolsBytoolidAuth200Response.md)

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

<a id="chatGetAgentsToolsCalls"></a>
# **chatGetAgentsToolsCalls**
> kotlin.Any chatGetAgentsToolsCalls()

Get tool call history

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
try {
    val result : kotlin.Any = apiInstance.chatGetAgentsToolsCalls()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatGetAgentsToolsCalls")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatGetAgentsToolsCalls")
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

<a id="chatPatchAgentsByid"></a>
# **chatPatchAgentsByid**
> ChatAgent chatPatchAgentsByid(id, chatAgentCreateParams)

Update an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
val chatAgentCreateParams : ChatAgentCreateParams =  // ChatAgentCreateParams | 
try {
    val result : ChatAgent = apiInstance.chatPatchAgentsByid(id, chatAgentCreateParams)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPatchAgentsByid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPatchAgentsByid")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatAgentCreateParams** | [**ChatAgentCreateParams**](ChatAgentCreateParams.md)|  | |

### Return type

[**ChatAgent**](ChatAgent.md)

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

<a id="chatPostAgents"></a>
# **chatPostAgents**
> ChatAgent chatPostAgents(chatAgentCreateParams)

Create an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val chatAgentCreateParams : ChatAgentCreateParams =  // ChatAgentCreateParams | 
try {
    val result : ChatAgent = apiInstance.chatPostAgents(chatAgentCreateParams)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgents")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatAgentCreateParams** | [**ChatAgentCreateParams**](ChatAgentCreateParams.md)|  | |

### Return type

[**ChatAgent**](ChatAgent.md)

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

<a id="chatPostAgentsByidDuplicate"></a>
# **chatPostAgentsByidDuplicate**
> ChatAgent chatPostAgentsByidDuplicate(id)

Duplicate an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ChatAgent = apiInstance.chatPostAgentsByidDuplicate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsByidDuplicate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsByidDuplicate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ChatAgent**](ChatAgent.md)

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

<a id="chatPostAgentsByidRevert"></a>
# **chatPostAgentsByidRevert**
> kotlin.Any chatPostAgentsByidRevert(id, chatPostAgentsByidRevertRequest)

Revert agent to a previous version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val id : kotlin.String = id_example // kotlin.String | 
val chatPostAgentsByidRevertRequest : ChatPostAgentsByidRevertRequest =  // ChatPostAgentsByidRevertRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAgentsByidRevert(id, chatPostAgentsByidRevertRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsByidRevert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsByidRevert")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsByidRevertRequest** | [**ChatPostAgentsByidRevertRequest**](ChatPostAgentsByidRevertRequest.md)|  | |

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

<a id="chatPostAgentsChat"></a>
# **chatPostAgentsChat**
> kotlin.String chatPostAgentsChat(chatAgentChatRequest)

Chat with an agent

Send a message to an agent and receive a streaming SSE response.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val chatAgentChatRequest : ChatAgentChatRequest =  // ChatAgentChatRequest | 
try {
    val result : kotlin.String = apiInstance.chatPostAgentsChat(chatAgentChatRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsChat")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsChat")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatAgentChatRequest** | [**ChatAgentChatRequest**](ChatAgentChatRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="chatPostAgentsChatAbort"></a>
# **chatPostAgentsChatAbort**
> ChatPostAgentsChatAbort200Response chatPostAgentsChatAbort(chatPostAgentsChatAbortRequest)

Abort an ongoing agent generation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val chatPostAgentsChatAbortRequest : ChatPostAgentsChatAbortRequest =  // ChatPostAgentsChatAbortRequest | 
try {
    val result : ChatPostAgentsChatAbort200Response = apiInstance.chatPostAgentsChatAbort(chatPostAgentsChatAbortRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsChatAbort")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsChatAbort")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsChatAbortRequest** | [**ChatPostAgentsChatAbortRequest**](ChatPostAgentsChatAbortRequest.md)|  | |

### Return type

[**ChatPostAgentsChatAbort200Response**](ChatPostAgentsChatAbort200Response.md)

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

<a id="chatPostAgentsChatByendpoint"></a>
# **chatPostAgentsChatByendpoint**
> kotlin.String chatPostAgentsChatByendpoint(endpoint, chatAgentChatRequest)

Chat with an ephemeral agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val endpoint : kotlin.String = endpoint_example // kotlin.String | 
val chatAgentChatRequest : ChatAgentChatRequest =  // ChatAgentChatRequest | 
try {
    val result : kotlin.String = apiInstance.chatPostAgentsChatByendpoint(endpoint, chatAgentChatRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsChatByendpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsChatByendpoint")
    e.printStackTrace()
}
```

### Parameters
| **endpoint** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatAgentChatRequest** | [**ChatAgentChatRequest**](ChatAgentChatRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="chatPostAgentsToolsBytoolidCall"></a>
# **chatPostAgentsToolsBytoolidCall**
> kotlin.Any chatPostAgentsToolsBytoolidCall(toolId, body)

Execute a tool call

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsApi()
val toolId : kotlin.String = toolId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostAgentsToolsBytoolidCall(toolId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsApi#chatPostAgentsToolsBytoolidCall")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsApi#chatPostAgentsToolsBytoolidCall")
    e.printStackTrace()
}
```

### Parameters
| **toolId** | **kotlin.String**|  | |
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

