# TasksApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchCancelTasks**](TasksApi.md#searchCancelTasks) | **POST** /v1/search/tasks/cancel | Cancel enqueued or processing tasks |
| [**searchDeleteTasks**](TasksApi.md#searchDeleteTasks) | **DELETE** /v1/search/tasks | Delete completed tasks |
| [**searchGetTask**](TasksApi.md#searchGetTask) | **GET** /v1/search/tasks/{taskUid} | Get task details |
| [**searchListTasks**](TasksApi.md#searchListTasks) | **GET** /v1/search/tasks | List all tasks |
| [**tasksTasksEvents**](TasksApi.md#tasksTasksEvents) | **GET** /v1/tasks/events | Realtime event stream (SSE, identity-gated) |
| [**tasksTasksGet**](TasksApi.md#tasksTasksGet) | **GET** /v1/tasks/{resource} | Engine JSON API (namespaces, workflows, activities, …), identity-gated |
| [**tasksTasksMcp**](TasksApi.md#tasksTasksMcp) | **POST** /v1/tasks/mcp | Tasks MCP tool surface (JSON-RPC, identity-gated) |
| [**tasksTasksPost**](TasksApi.md#tasksTasksPost) | **POST** /v1/tasks/{resource} | Engine JSON API write (identity-gated) |


<a id="searchCancelTasks"></a>
# **searchCancelTasks**
> SearchSummarizedTaskView searchCancelTasks(uids, statuses, types, indexUids)

Cancel enqueued or processing tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val uids : kotlin.String = uids_example // kotlin.String | 
val statuses : kotlin.String = statuses_example // kotlin.String | 
val types : kotlin.String = types_example // kotlin.String | 
val indexUids : kotlin.String = indexUids_example // kotlin.String | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchCancelTasks(uids, statuses, types, indexUids)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#searchCancelTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#searchCancelTasks")
    e.printStackTrace()
}
```

### Parameters
| **uids** | **kotlin.String**|  | [optional] |
| **statuses** | **kotlin.String**|  | [optional] |
| **types** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUids** | **kotlin.String**|  | [optional] |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="searchDeleteTasks"></a>
# **searchDeleteTasks**
> SearchSummarizedTaskView searchDeleteTasks(uids, statuses, types, indexUids)

Delete completed tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val uids : kotlin.String = uids_example // kotlin.String | 
val statuses : kotlin.String = statuses_example // kotlin.String | 
val types : kotlin.String = types_example // kotlin.String | 
val indexUids : kotlin.String = indexUids_example // kotlin.String | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteTasks(uids, statuses, types, indexUids)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#searchDeleteTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#searchDeleteTasks")
    e.printStackTrace()
}
```

### Parameters
| **uids** | **kotlin.String**|  | [optional] |
| **statuses** | **kotlin.String**|  | [optional] |
| **types** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUids** | **kotlin.String**|  | [optional] |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="searchGetTask"></a>
# **searchGetTask**
> SearchTaskView searchGetTask(taskUid)

Get task details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val taskUid : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : SearchTaskView = apiInstance.searchGetTask(taskUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#searchGetTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#searchGetTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **taskUid** | **kotlin.Int**|  | |

### Return type

[**SearchTaskView**](SearchTaskView.md)

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

<a id="searchListTasks"></a>
# **searchListTasks**
> SearchListTasks200Response searchListTasks(limit, from, uids, statuses, types, indexUids)

List all tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
val from : kotlin.Int = 56 // kotlin.Int | Task UID to start from
val uids : kotlin.String = uids_example // kotlin.String | Comma-separated task UIDs
val statuses : kotlin.String = statuses_example // kotlin.String | Comma-separated statuses (enqueued, processing, succeeded, failed, canceled)
val types : kotlin.String = types_example // kotlin.String | Comma-separated task types
val indexUids : kotlin.String = indexUids_example // kotlin.String | Comma-separated index UIDs
try {
    val result : SearchListTasks200Response = apiInstance.searchListTasks(limit, from, uids, statuses, types, indexUids)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#searchListTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#searchListTasks")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |
| **from** | **kotlin.Int**| Task UID to start from | [optional] |
| **uids** | **kotlin.String**| Comma-separated task UIDs | [optional] |
| **statuses** | **kotlin.String**| Comma-separated statuses (enqueued, processing, succeeded, failed, canceled) | [optional] |
| **types** | **kotlin.String**| Comma-separated task types | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUids** | **kotlin.String**| Comma-separated index UIDs | [optional] |

### Return type

[**SearchListTasks200Response**](SearchListTasks200Response.md)

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

<a id="tasksTasksEvents"></a>
# **tasksTasksEvents**
> kotlin.String tasksTasksEvents()

Realtime event stream (SSE, identity-gated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
try {
    val result : kotlin.String = apiInstance.tasksTasksEvents()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#tasksTasksEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#tasksTasksEvents")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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
 - **Accept**: application/json

<a id="tasksTasksGet"></a>
# **tasksTasksGet**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksGet(resource)

Engine JSON API (namespaces, workflows, activities, …), identity-gated

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val resource : kotlin.String = resource_example // kotlin.String | 'Engine resource path (e.g. namespaces, nexus)'
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksGet(resource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#tasksTasksGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#tasksTasksGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resource** | **kotlin.String**| &#39;Engine resource path (e.g. namespaces, nexus)&#39; | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="tasksTasksMcp"></a>
# **tasksTasksMcp**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksMcp(requestBody)

Tasks MCP tool surface (JSON-RPC, identity-gated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val requestBody : kotlin.collections.Map<kotlin.String, kotlin.Any?> = Object // kotlin.collections.Map<kotlin.String, kotlin.Any?> | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksMcp(requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#tasksTasksMcp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#tasksTasksMcp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any?&gt;**](kotlin.Any.md)|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="tasksTasksPost"></a>
# **tasksTasksPost**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksPost(resource, requestBody)

Engine JSON API write (identity-gated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TasksApi()
val resource : kotlin.String = resource_example // kotlin.String | 
val requestBody : kotlin.collections.Map<kotlin.String, kotlin.Any> = Object // kotlin.collections.Map<kotlin.String, kotlin.Any> | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksPost(resource, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TasksApi#tasksTasksPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TasksApi#tasksTasksPost")
    e.printStackTrace()
}
```

### Parameters
| **resource** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

