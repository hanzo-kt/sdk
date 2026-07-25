# AgentSessionsAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudAgentSessionsControllerAppendEvent**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerAppendEvent) | **POST** /v1/agents/sessions/{id}/events |  |
| [**cloudAgentSessionsControllerGet**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerGet) | **GET** /v1/agents/sessions/{id} |  |
| [**cloudAgentSessionsControllerList**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerList) | **GET** /v1/agents/sessions |  |
| [**cloudAgentSessionsControllerMessage**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerMessage) | **POST** /v1/agents/sessions/{id}/message |  |
| [**cloudAgentSessionsControllerPatch**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerPatch) | **PATCH** /v1/agents/sessions/{id} |  |
| [**cloudAgentSessionsControllerPause**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerPause) | **POST** /v1/agents/sessions/{id}/pause |  |
| [**cloudAgentSessionsControllerRegister**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerRegister) | **POST** /v1/agents/sessions |  |
| [**cloudAgentSessionsControllerResume**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerResume) | **POST** /v1/agents/sessions/{id}/resume |  |
| [**cloudAgentSessionsControllerStop**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerStop) | **POST** /v1/agents/sessions/{id}/stop |  |
| [**cloudAgentSessionsControllerStream**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerStream) | **GET** /v1/agents/sessions/stream |  |
| [**cloudAgentSessionsControllerTree**](AgentSessionsAPIApi.md#cloudAgentSessionsControllerTree) | **GET** /v1/agents/sessions/{id}/tree |  |


<a id="cloudAgentSessionsControllerAppendEvent"></a>
# **cloudAgentSessionsControllerAppendEvent**
> CloudAgentsEvent cloudAgentSessionsControllerAppendEvent(id, cloudAgentsEventRequest)



Append one event to a session&#39;s ordered log (a model message, tool call, subagent spawn, free log line, status change, or control command). Seq is allocated monotonically per session. The payload is an opaque, size-bounded, well-formed JSON blob.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val cloudAgentsEventRequest : CloudAgentsEventRequest =  // CloudAgentsEventRequest | 
try {
    val result : CloudAgentsEvent = apiInstance.cloudAgentSessionsControllerAppendEvent(id, cloudAgentsEventRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerAppendEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerAppendEvent")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsEventRequest** | [**CloudAgentsEventRequest**](CloudAgentsEventRequest.md)|  | |

### Return type

[**CloudAgentsEvent**](CloudAgentsEvent.md)

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

<a id="cloudAgentSessionsControllerGet"></a>
# **cloudAgentSessionsControllerGet**
> CloudAgentsSessionDetail cloudAgentSessionsControllerGet(id)



Session detail — the session, its direct child sessions, and up to 50 recent events.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
try {
    val result : CloudAgentsSessionDetail = apiInstance.cloudAgentSessionsControllerGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The session id (sess_...). | |

### Return type

[**CloudAgentsSessionDetail**](CloudAgentsSessionDetail.md)

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

<a id="cloudAgentSessionsControllerList"></a>
# **cloudAgentSessionsControllerList**
> CloudAgentSessionsControllerList200Response cloudAgentSessionsControllerList(root, parent, status, limit)



List the org&#39;s live sessions, newest first. With no filter only roots (the outer-agent view) are returned; root scopes to one tree, parent to a session&#39;s direct children.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val root : kotlin.String = root_example // kotlin.String | Return every session in this tree (rootSessionId == root).
val parent : kotlin.String = parent_example // kotlin.String | Return the direct children of this session.
val status : kotlin.String = status_example // kotlin.String | Filter by status.
val limit : kotlin.Int = 56 // kotlin.Int | Max sessions to return (default 100, max 500).
try {
    val result : CloudAgentSessionsControllerList200Response = apiInstance.cloudAgentSessionsControllerList(root, parent, status, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerList")
    e.printStackTrace()
}
```

### Parameters
| **root** | **kotlin.String**| Return every session in this tree (rootSessionId &#x3D;&#x3D; root). | [optional] |
| **parent** | **kotlin.String**| Return the direct children of this session. | [optional] |
| **status** | **kotlin.String**| Filter by status. | [optional] [enum: running, paused, done, error] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max sessions to return (default 100, max 500). | [optional] |

### Return type

[**CloudAgentSessionsControllerList200Response**](CloudAgentSessionsControllerList200Response.md)

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

<a id="cloudAgentSessionsControllerMessage"></a>
# **cloudAgentSessionsControllerMessage**
> CloudAgentsControlResult cloudAgentSessionsControllerMessage(id, cloudAgentsControlRequest)



Send a steering message to a live session. Requires a &#39;message&#39; or &#39;payload&#39;. Records a durable control event and forwards to the tasks engine when the session is task-backed.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val cloudAgentsControlRequest : CloudAgentsControlRequest =  // CloudAgentsControlRequest | 
try {
    val result : CloudAgentsControlResult = apiInstance.cloudAgentSessionsControllerMessage(id, cloudAgentsControlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerMessage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsControlRequest** | [**CloudAgentsControlRequest**](CloudAgentsControlRequest.md)|  | |

### Return type

[**CloudAgentsControlResult**](CloudAgentsControlResult.md)

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

<a id="cloudAgentSessionsControllerPatch"></a>
# **cloudAgentSessionsControllerPatch**
> CloudAgentsSession cloudAgentSessionsControllerPatch(id, agentsPatchSessionRequest)



Update a session&#39;s status and/or title. A terminal session (done/error) is monotonic — it cannot be reopened.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val agentsPatchSessionRequest : AgentsPatchSessionRequest =  // AgentsPatchSessionRequest | 
try {
    val result : CloudAgentsSession = apiInstance.cloudAgentSessionsControllerPatch(id, agentsPatchSessionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerPatch")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **agentsPatchSessionRequest** | [**AgentsPatchSessionRequest**](AgentsPatchSessionRequest.md)|  | |

### Return type

[**CloudAgentsSession**](CloudAgentsSession.md)

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

<a id="cloudAgentSessionsControllerPause"></a>
# **cloudAgentSessionsControllerPause**
> CloudAgentsControlResult cloudAgentSessionsControllerPause(id, cloudAgentsControlRequest)



Pause a live session. Records a durable control event and, when the session is backed by a hanzoai/tasks workflow and a tasks backend is wired, forwards the command to the engine&#39;s signal API.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val cloudAgentsControlRequest : CloudAgentsControlRequest =  // CloudAgentsControlRequest | 
try {
    val result : CloudAgentsControlResult = apiInstance.cloudAgentSessionsControllerPause(id, cloudAgentsControlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerPause")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerPause")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsControlRequest** | [**CloudAgentsControlRequest**](CloudAgentsControlRequest.md)|  | [optional] |

### Return type

[**CloudAgentsControlResult**](CloudAgentsControlResult.md)

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

<a id="cloudAgentSessionsControllerRegister"></a>
# **cloudAgentSessionsControllerRegister**
> CloudAgentsSession cloudAgentSessionsControllerRegister(agentsRegisterSessionRequest)



Register a live agent session. With no parentSessionId the session is a root (the outer agent); with one it is a subagent child of that parent (which must exist in the same org) and inherits its rootSessionId — the tree key every node in one flow shares.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val agentsRegisterSessionRequest : AgentsRegisterSessionRequest =  // AgentsRegisterSessionRequest | 
try {
    val result : CloudAgentsSession = apiInstance.cloudAgentSessionsControllerRegister(agentsRegisterSessionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerRegister")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerRegister")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **agentsRegisterSessionRequest** | [**AgentsRegisterSessionRequest**](AgentsRegisterSessionRequest.md)|  | |

### Return type

[**CloudAgentsSession**](CloudAgentsSession.md)

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

<a id="cloudAgentSessionsControllerResume"></a>
# **cloudAgentSessionsControllerResume**
> CloudAgentsControlResult cloudAgentSessionsControllerResume(id, cloudAgentsControlRequest)



Resume a paused session. Records a durable control event and forwards to the tasks engine when the session is task-backed.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val cloudAgentsControlRequest : CloudAgentsControlRequest =  // CloudAgentsControlRequest | 
try {
    val result : CloudAgentsControlResult = apiInstance.cloudAgentSessionsControllerResume(id, cloudAgentsControlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerResume")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerResume")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsControlRequest** | [**CloudAgentsControlRequest**](CloudAgentsControlRequest.md)|  | [optional] |

### Return type

[**CloudAgentsControlResult**](CloudAgentsControlResult.md)

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

<a id="cloudAgentSessionsControllerStop"></a>
# **cloudAgentSessionsControllerStop**
> CloudAgentsControlResult cloudAgentSessionsControllerStop(id, cloudAgentsControlRequest)



Stop a session. Records a durable control event and, when task-backed, cancels the underlying hanzoai/tasks workflow.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
val cloudAgentsControlRequest : CloudAgentsControlRequest =  // CloudAgentsControlRequest | 
try {
    val result : CloudAgentsControlResult = apiInstance.cloudAgentSessionsControllerStop(id, cloudAgentsControlRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerStop")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerStop")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The session id (sess_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsControlRequest** | [**CloudAgentsControlRequest**](CloudAgentsControlRequest.md)|  | [optional] |

### Return type

[**CloudAgentsControlResult**](CloudAgentsControlResult.md)

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

<a id="cloudAgentSessionsControllerStream"></a>
# **cloudAgentSessionsControllerStream**
> kotlin.String cloudAgentSessionsControllerStream(root)



Server-Sent Events feed of live session + event updates for the caller&#39;s org (streams natively over the ZAP machine transport as well). Optional ?root scopes the feed to one subagent tree. Each frame carries an event type (session or event) and a JSON data line; the GET list/detail/tree endpoints remain the source of truth, the stream is a live hint.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val root : kotlin.String = root_example // kotlin.String | Scope the feed to one subagent tree (rootSessionId).
try {
    val result : kotlin.String = apiInstance.cloudAgentSessionsControllerStream(root)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerStream")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerStream")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **root** | **kotlin.String**| Scope the feed to one subagent tree (rootSessionId). | [optional] |

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

<a id="cloudAgentSessionsControllerTree"></a>
# **cloudAgentSessionsControllerTree**
> CloudAgentsTreeNode cloudAgentSessionsControllerTree(id)



The full subagent-flow graph rooted at this session&#39;s tree — each node is a session plus its children, recursively, with real per-node event and fan-out counts.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentSessionsAPIApi()
val id : kotlin.String = id_example // kotlin.String | The session id (sess_...).
try {
    val result : CloudAgentsTreeNode = apiInstance.cloudAgentSessionsControllerTree(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerTree")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentSessionsAPIApi#cloudAgentSessionsControllerTree")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The session id (sess_...). | |

### Return type

[**CloudAgentsTreeNode**](CloudAgentsTreeNode.md)

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

