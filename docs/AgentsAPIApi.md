# AgentsAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudAgentsControllerActivity**](AgentsAPIApi.md#cloudAgentsControllerActivity) | **GET** /v1/agents/activity |  |
| [**cloudAgentsControllerCreate**](AgentsAPIApi.md#cloudAgentsControllerCreate) | **POST** /v1/agents |  |
| [**cloudAgentsControllerDelete**](AgentsAPIApi.md#cloudAgentsControllerDelete) | **DELETE** /v1/agents/{ref} |  |
| [**cloudAgentsControllerGet**](AgentsAPIApi.md#cloudAgentsControllerGet) | **GET** /v1/agents/{ref} |  |
| [**cloudAgentsControllerList**](AgentsAPIApi.md#cloudAgentsControllerList) | **GET** /v1/agents |  |
| [**cloudAgentsControllerMetrics**](AgentsAPIApi.md#cloudAgentsControllerMetrics) | **GET** /v1/agents/metrics |  |
| [**cloudAgentsControllerRun**](AgentsAPIApi.md#cloudAgentsControllerRun) | **POST** /v1/agents/{ref}/run |  |
| [**cloudAgentsControllerRuns**](AgentsAPIApi.md#cloudAgentsControllerRuns) | **GET** /v1/agents/{ref}/runs |  |
| [**cloudAgentsControllerUpdate**](AgentsAPIApi.md#cloudAgentsControllerUpdate) | **PATCH** /v1/agents/{ref} |  |


<a id="cloudAgentsControllerActivity"></a>
# **cloudAgentsControllerActivity**
> CloudAgentsControllerActivity200Response cloudAgentsControllerActivity()



The org-wide recent-activity feed (newest first, capped at 50). Each recorded run is an invoked/failed event; each agent&#39;s own create/update timestamps are created/updated events. Nothing is invented.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
try {
    val result : CloudAgentsControllerActivity200Response = apiInstance.cloudAgentsControllerActivity()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerActivity")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudAgentsControllerActivity200Response**](CloudAgentsControllerActivity200Response.md)

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

<a id="cloudAgentsControllerCreate"></a>
# **cloudAgentsControllerCreate**
> CloudAgentsAgent cloudAgentsControllerCreate(cloudAgentsCreateAgentRequest)



Create an agent (a model + instructions + tool names). A long-running agent additionally requires a 5-field cron &#39;schedule&#39; and is invoked by the scheduler; a one-shot agent runs only when POSTed to /run.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val cloudAgentsCreateAgentRequest : CloudAgentsCreateAgentRequest =  // CloudAgentsCreateAgentRequest | 
try {
    val result : CloudAgentsAgent = apiInstance.cloudAgentsControllerCreate(cloudAgentsCreateAgentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudAgentsCreateAgentRequest** | [**CloudAgentsCreateAgentRequest**](CloudAgentsCreateAgentRequest.md)|  | |

### Return type

[**CloudAgentsAgent**](CloudAgentsAgent.md)

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

<a id="cloudAgentsControllerDelete"></a>
# **cloudAgentsControllerDelete**
> cloudAgentsControllerDelete(ref)



Delete an agent and its run history.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val ref : kotlin.String = ref_example // kotlin.String | The agent's public id (agent_...) or org-unique name.
try {
    apiInstance.cloudAgentsControllerDelete(ref)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ref** | **kotlin.String**| The agent&#39;s public id (agent_...) or org-unique name. | |

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

<a id="cloudAgentsControllerGet"></a>
# **cloudAgentsControllerGet**
> CloudAgentsAgentDetail cloudAgentsControllerGet(ref)



Get an agent by its public id (agent_...) or org-unique name, with its instructions and up to 20 recent runs.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val ref : kotlin.String = ref_example // kotlin.String | The agent's public id (agent_...) or org-unique name.
try {
    val result : CloudAgentsAgentDetail = apiInstance.cloudAgentsControllerGet(ref)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ref** | **kotlin.String**| The agent&#39;s public id (agent_...) or org-unique name. | |

### Return type

[**CloudAgentsAgentDetail**](CloudAgentsAgentDetail.md)

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

<a id="cloudAgentsControllerList"></a>
# **cloudAgentsControllerList**
> CloudAgentsControllerList200Response cloudAgentsControllerList()



List the org&#39;s agents (most-recently-updated first).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
try {
    val result : CloudAgentsControllerList200Response = apiInstance.cloudAgentsControllerList()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerList")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudAgentsControllerList200Response**](CloudAgentsControllerList200Response.md)

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

<a id="cloudAgentsControllerMetrics"></a>
# **cloudAgentsControllerMetrics**
> CloudAgentsMetrics cloudAgentsControllerMetrics(range)



Invocations-over-time histogram for the org&#39;s Agents dashboard. Every point is a real count of recorded runs in that bucket, one series line per agent that ran in the window. The Resource Usage rollup is all-null (this store meters no CPU/memory/storage/cost).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val range : kotlin.String = range_example // kotlin.String | Window token; one of 24H, 7D, 30D (default 30D).
try {
    val result : CloudAgentsMetrics = apiInstance.cloudAgentsControllerMetrics(range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerMetrics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**| Window token; one of 24H, 7D, 30D (default 30D). | [optional] [enum: 24H, 7D, 30D] |

### Return type

[**CloudAgentsMetrics**](CloudAgentsMetrics.md)

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

<a id="cloudAgentsControllerRun"></a>
# **cloudAgentsControllerRun**
> CloudAgentsRun cloudAgentsControllerRun(ref, agentsRunRequest)



Run the agent — composes its instructions with the caller input and executes one real chat completion through the in-process AI client, records the run, and returns the run view. Requires a validated principal (money path). The org&#39;s credit balance is pre-authorized before any inference (fail-closed); a successful run debits a flat per-run fee metered as product&#x3D;agent. Duration is recorded; the run is real.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val ref : kotlin.String = ref_example // kotlin.String | The agent's public id (agent_...) or org-unique name.
val agentsRunRequest : AgentsRunRequest =  // AgentsRunRequest | 
try {
    val result : CloudAgentsRun = apiInstance.cloudAgentsControllerRun(ref, agentsRunRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerRun")
    e.printStackTrace()
}
```

### Parameters
| **ref** | **kotlin.String**| The agent&#39;s public id (agent_...) or org-unique name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **agentsRunRequest** | [**AgentsRunRequest**](AgentsRunRequest.md)|  | [optional] |

### Return type

[**CloudAgentsRun**](CloudAgentsRun.md)

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

<a id="cloudAgentsControllerRuns"></a>
# **cloudAgentsControllerRuns**
> CloudAgentsControllerRuns200Response cloudAgentsControllerRuns(ref, limit)



The agent&#39;s run history, newest first.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val ref : kotlin.String = ref_example // kotlin.String | The agent's public id (agent_...) or org-unique name.
val limit : kotlin.Int = 56 // kotlin.Int | Max runs to return (default 50, max 200).
try {
    val result : CloudAgentsControllerRuns200Response = apiInstance.cloudAgentsControllerRuns(ref, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerRuns")
    e.printStackTrace()
}
```

### Parameters
| **ref** | **kotlin.String**| The agent&#39;s public id (agent_...) or org-unique name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max runs to return (default 50, max 200). | [optional] |

### Return type

[**CloudAgentsControllerRuns200Response**](CloudAgentsControllerRuns200Response.md)

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

<a id="cloudAgentsControllerUpdate"></a>
# **cloudAgentsControllerUpdate**
> CloudAgentsAgent cloudAgentsControllerUpdate(ref, agentsUpdateAgentRequest)



Update an agent&#39;s mutable fields. The resulting execution mode + schedule are re-validated, so a partial update can never leave a long-running agent without a valid cron.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AgentsAPIApi()
val ref : kotlin.String = ref_example // kotlin.String | The agent's public id (agent_...) or org-unique name.
val agentsUpdateAgentRequest : AgentsUpdateAgentRequest =  // AgentsUpdateAgentRequest | 
try {
    val result : CloudAgentsAgent = apiInstance.cloudAgentsControllerUpdate(ref, agentsUpdateAgentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AgentsAPIApi#cloudAgentsControllerUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AgentsAPIApi#cloudAgentsControllerUpdate")
    e.printStackTrace()
}
```

### Parameters
| **ref** | **kotlin.String**| The agent&#39;s public id (agent_...) or org-unique name. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **agentsUpdateAgentRequest** | [**AgentsUpdateAgentRequest**](AgentsUpdateAgentRequest.md)|  | |

### Return type

[**CloudAgentsAgent**](CloudAgentsAgent.md)

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

