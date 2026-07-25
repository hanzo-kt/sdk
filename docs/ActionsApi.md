# ActionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatDeleteAgentsActionsByagentIdByactionId**](ActionsApi.md#chatDeleteAgentsActionsByagentIdByactionId) | **DELETE** /v1/chat/agents/actions/{agent_id}/{action_id} | Delete an agent action |
| [**chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel**](ActionsApi.md#chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel) | **DELETE** /v1/chat/assistants/v1/actions/{assistant_id}/{action_id}/{model} | Delete an assistant action (v1) |
| [**chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel**](ActionsApi.md#chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel) | **DELETE** /v1/chat/assistants/v2/actions/{assistant_id}/{action_id}/{model} | Delete an assistant action (v2) |
| [**chatGetActionsByactionIdOauthCallback**](ActionsApi.md#chatGetActionsByactionIdOauthCallback) | **GET** /v1/chat/actions/{action_id}/oauth/callback | Action OAuth callback |
| [**chatGetAgentsActions**](ActionsApi.md#chatGetAgentsActions) | **GET** /v1/chat/agents/actions | List agent actions |
| [**chatPostActionsByactionIdOauthBind**](ActionsApi.md#chatPostActionsByactionIdOauthBind) | **POST** /v1/chat/actions/{action_id}/oauth/bind | Set CSRF cookie for action OAuth flow |
| [**chatPostAgentsActionsByagentId**](ActionsApi.md#chatPostAgentsActionsByagentId) | **POST** /v1/chat/agents/actions/{agent_id} | Add or update actions for an agent |
| [**chatPostAssistantsV1ActionsByassistantId**](ActionsApi.md#chatPostAssistantsV1ActionsByassistantId) | **POST** /v1/chat/assistants/v1/actions/{assistant_id} | Add or update actions for an assistant (v1) |
| [**chatPostAssistantsV2ActionsByassistantId**](ActionsApi.md#chatPostAssistantsV2ActionsByassistantId) | **POST** /v1/chat/assistants/v2/actions/{assistant_id} | Add or update actions for an assistant (v2) |


<a id="chatDeleteAgentsActionsByagentIdByactionId"></a>
# **chatDeleteAgentsActionsByagentIdByactionId**
> kotlin.Any chatDeleteAgentsActionsByagentIdByactionId(agentId, actionId)

Delete an agent action

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val agentId : kotlin.String = agentId_example // kotlin.String | 
val actionId : kotlin.String = actionId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAgentsActionsByagentIdByactionId(agentId, actionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatDeleteAgentsActionsByagentIdByactionId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatDeleteAgentsActionsByagentIdByactionId")
    e.printStackTrace()
}
```

### Parameters
| **agentId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **actionId** | **kotlin.String**|  | |

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

<a id="chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel"></a>
# **chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel**
> kotlin.Any chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel(assistantId, actionId, model)

Delete an assistant action (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val actionId : kotlin.String = actionId_example // kotlin.String | 
val model : kotlin.String = model_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel(assistantId, actionId, model)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatDeleteAssistantsV1ActionsByassistantIdByactionIdBymodel")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
| **actionId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **model** | **kotlin.String**|  | |

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

<a id="chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel"></a>
# **chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel**
> kotlin.Any chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel(assistantId, actionId, model)

Delete an assistant action (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val actionId : kotlin.String = actionId_example // kotlin.String | 
val model : kotlin.String = model_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel(assistantId, actionId, model)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatDeleteAssistantsV2ActionsByassistantIdByactionIdBymodel")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
| **actionId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **model** | **kotlin.String**|  | |

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

<a id="chatGetActionsByactionIdOauthCallback"></a>
# **chatGetActionsByactionIdOauthCallback**
> chatGetActionsByactionIdOauthCallback(actionId, code, state)

Action OAuth callback

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val actionId : kotlin.String = actionId_example // kotlin.String | 
val code : kotlin.String = code_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
try {
    apiInstance.chatGetActionsByactionIdOauthCallback(actionId, code, state)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatGetActionsByactionIdOauthCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatGetActionsByactionIdOauthCallback")
    e.printStackTrace()
}
```

### Parameters
| **actionId** | **kotlin.String**|  | |
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

<a id="chatGetAgentsActions"></a>
# **chatGetAgentsActions**
> kotlin.collections.List&lt;ChatAction&gt; chatGetAgentsActions()

List agent actions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
try {
    val result : kotlin.collections.List<ChatAction> = apiInstance.chatGetAgentsActions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatGetAgentsActions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatGetAgentsActions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ChatAction&gt;**](ChatAction.md)

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

<a id="chatPostActionsByactionIdOauthBind"></a>
# **chatPostActionsByactionIdOauthBind**
> kotlin.Any chatPostActionsByactionIdOauthBind(actionId)

Set CSRF cookie for action OAuth flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val actionId : kotlin.String = actionId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatPostActionsByactionIdOauthBind(actionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatPostActionsByactionIdOauthBind")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatPostActionsByactionIdOauthBind")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **actionId** | **kotlin.String**|  | |

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

<a id="chatPostAgentsActionsByagentId"></a>
# **chatPostAgentsActionsByagentId**
> kotlin.Any chatPostAgentsActionsByagentId(agentId, chatPostAgentsActionsByagentIdRequest)

Add or update actions for an agent

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val agentId : kotlin.String = agentId_example // kotlin.String | 
val chatPostAgentsActionsByagentIdRequest : ChatPostAgentsActionsByagentIdRequest =  // ChatPostAgentsActionsByagentIdRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAgentsActionsByagentId(agentId, chatPostAgentsActionsByagentIdRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatPostAgentsActionsByagentId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatPostAgentsActionsByagentId")
    e.printStackTrace()
}
```

### Parameters
| **agentId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsActionsByagentIdRequest** | [**ChatPostAgentsActionsByagentIdRequest**](ChatPostAgentsActionsByagentIdRequest.md)|  | |

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

<a id="chatPostAssistantsV1ActionsByassistantId"></a>
# **chatPostAssistantsV1ActionsByassistantId**
> kotlin.Any chatPostAssistantsV1ActionsByassistantId(assistantId, chatPostAgentsActionsByagentIdRequest)

Add or update actions for an assistant (v1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val chatPostAgentsActionsByagentIdRequest : ChatPostAgentsActionsByagentIdRequest =  // ChatPostAgentsActionsByagentIdRequest | 
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV1ActionsByassistantId(assistantId, chatPostAgentsActionsByagentIdRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatPostAssistantsV1ActionsByassistantId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatPostAssistantsV1ActionsByassistantId")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **chatPostAgentsActionsByagentIdRequest** | [**ChatPostAgentsActionsByagentIdRequest**](ChatPostAgentsActionsByagentIdRequest.md)|  | |

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

<a id="chatPostAssistantsV2ActionsByassistantId"></a>
# **chatPostAssistantsV2ActionsByassistantId**
> kotlin.Any chatPostAssistantsV2ActionsByassistantId(assistantId, body)

Add or update actions for an assistant (v2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActionsApi()
val assistantId : kotlin.String = assistantId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostAssistantsV2ActionsByassistantId(assistantId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActionsApi#chatPostAssistantsV2ActionsByassistantId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActionsApi#chatPostAssistantsV2ActionsByassistantId")
    e.printStackTrace()
}
```

### Parameters
| **assistantId** | **kotlin.String**|  | |
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

