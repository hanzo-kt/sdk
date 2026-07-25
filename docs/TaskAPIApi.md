# TaskAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddTask**](TaskAPIApi.md#cloudApiControllerAddTask) | **POST** /v1/cloud/add-task | Api Controller Add Task |
| [**cloudApiControllerDeleteTask**](TaskAPIApi.md#cloudApiControllerDeleteTask) | **POST** /v1/cloud/delete-task | Api Controller Delete Task |
| [**cloudApiControllerGetGlobalTasks**](TaskAPIApi.md#cloudApiControllerGetGlobalTasks) | **GET** /v1/cloud/get-global-tasks | Api Controller Get Global Tasks |
| [**cloudApiControllerGetTask**](TaskAPIApi.md#cloudApiControllerGetTask) | **GET** /v1/cloud/get-task | Api Controller Get Task |
| [**cloudApiControllerGetTasks**](TaskAPIApi.md#cloudApiControllerGetTasks) | **GET** /v1/cloud/get-tasks | Api Controller Get Tasks |
| [**cloudApiControllerUpdateTask**](TaskAPIApi.md#cloudApiControllerUpdateTask) | **POST** /v1/cloud/update-task | Api Controller Update Task |
| [**nexusAddTask**](TaskAPIApi.md#nexusAddTask) | **POST** /v1/nexus/add-task | add Task |
| [**nexusDeleteTask**](TaskAPIApi.md#nexusDeleteTask) | **POST** /v1/nexus/delete-task | delete Task |
| [**nexusGetGlobalTasks**](TaskAPIApi.md#nexusGetGlobalTasks) | **GET** /v1/nexus/get-global-tasks | get Global Tasks |
| [**nexusGetTask**](TaskAPIApi.md#nexusGetTask) | **GET** /v1/nexus/get-task | get Task |
| [**nexusGetTasks**](TaskAPIApi.md#nexusGetTasks) | **GET** /v1/nexus/get-tasks | get Tasks |
| [**nexusUpdateTask**](TaskAPIApi.md#nexusUpdateTask) | **POST** /v1/nexus/update-task | update Task |


<a id="cloudApiControllerAddTask"></a>
# **cloudApiControllerAddTask**
> CloudControllersResponse cloudApiControllerAddTask(cloudObjectTask)

Api Controller Add Task

add task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val cloudObjectTask : CloudObjectTask =  // CloudObjectTask | The details of the task
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddTask(cloudObjectTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerAddTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerAddTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTask** | [**CloudObjectTask**](CloudObjectTask.md)| The details of the task | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteTask"></a>
# **cloudApiControllerDeleteTask**
> CloudControllersResponse cloudApiControllerDeleteTask(cloudObjectTask)

Api Controller Delete Task

delete task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val cloudObjectTask : CloudObjectTask =  // CloudObjectTask | The details of the task
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteTask(cloudObjectTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerDeleteTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerDeleteTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTask** | [**CloudObjectTask**](CloudObjectTask.md)| The details of the task | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetGlobalTasks"></a>
# **cloudApiControllerGetGlobalTasks**
> kotlin.collections.List&lt;CloudObjectTask&gt; cloudApiControllerGetGlobalTasks()

Api Controller Get Global Tasks

get global tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectTask> = apiInstance.cloudApiControllerGetGlobalTasks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerGetGlobalTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerGetGlobalTasks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectTask&gt;**](CloudObjectTask.md)

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

<a id="cloudApiControllerGetTask"></a>
# **cloudApiControllerGetTask**
> CloudObjectTask cloudApiControllerGetTask(id)

Api Controller Get Task

get task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of task
try {
    val result : CloudObjectTask = apiInstance.cloudApiControllerGetTask(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerGetTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerGetTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of task | |

### Return type

[**CloudObjectTask**](CloudObjectTask.md)

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

<a id="cloudApiControllerGetTasks"></a>
# **cloudApiControllerGetTasks**
> kotlin.collections.List&lt;CloudObjectTask&gt; cloudApiControllerGetTasks(owner)

Api Controller Get Tasks

get tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of task
try {
    val result : kotlin.collections.List<CloudObjectTask> = apiInstance.cloudApiControllerGetTasks(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerGetTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerGetTasks")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of task | |

### Return type

[**kotlin.collections.List&lt;CloudObjectTask&gt;**](CloudObjectTask.md)

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

<a id="cloudApiControllerUpdateTask"></a>
# **cloudApiControllerUpdateTask**
> CloudControllersResponse cloudApiControllerUpdateTask(id, cloudObjectTask)

Api Controller Update Task

update task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the task
val cloudObjectTask : CloudObjectTask =  // CloudObjectTask | The details of the task
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateTask(id, cloudObjectTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#cloudApiControllerUpdateTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#cloudApiControllerUpdateTask")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the task | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTask** | [**CloudObjectTask**](CloudObjectTask.md)| The details of the task | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddTask"></a>
# **nexusAddTask**
> NexusResponse nexusAddTask(nexusTask)

add Task

Add a task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val nexusTask : NexusTask =  // NexusTask | The details of the task
try {
    val result : NexusResponse = apiInstance.nexusAddTask(nexusTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusAddTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusAddTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusTask** | [**NexusTask**](NexusTask.md)| The details of the task | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteTask"></a>
# **nexusDeleteTask**
> NexusResponse nexusDeleteTask(nexusTask)

delete Task

Delete a task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val nexusTask : NexusTask =  // NexusTask | The details of the task
try {
    val result : NexusResponse = apiInstance.nexusDeleteTask(nexusTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusDeleteTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusDeleteTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusTask** | [**NexusTask**](NexusTask.md)| The details of the task | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetGlobalTasks"></a>
# **nexusGetGlobalTasks**
> kotlin.collections.List&lt;NexusTask&gt; nexusGetGlobalTasks()

get Global Tasks

Get global tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
try {
    val result : kotlin.collections.List<NexusTask> = apiInstance.nexusGetGlobalTasks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusGetGlobalTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusGetGlobalTasks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusTask&gt;**](NexusTask.md)

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

<a id="nexusGetTask"></a>
# **nexusGetTask**
> NexusTask nexusGetTask(id)

get Task

Get a task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the task
try {
    val result : NexusTask = apiInstance.nexusGetTask(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusGetTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusGetTask")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the task | |

### Return type

[**NexusTask**](NexusTask.md)

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

<a id="nexusGetTasks"></a>
# **nexusGetTasks**
> kotlin.collections.List&lt;NexusTask&gt; nexusGetTasks(owner)

get Tasks

Get tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the tasks
try {
    val result : kotlin.collections.List<NexusTask> = apiInstance.nexusGetTasks(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusGetTasks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusGetTasks")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the tasks | |

### Return type

[**kotlin.collections.List&lt;NexusTask&gt;**](NexusTask.md)

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

<a id="nexusUpdateTask"></a>
# **nexusUpdateTask**
> NexusResponse nexusUpdateTask(id, nexusTask)

update Task

Update a task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TaskAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the task
val nexusTask : NexusTask =  // NexusTask | The details of the task
try {
    val result : NexusResponse = apiInstance.nexusUpdateTask(id, nexusTask)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TaskAPIApi#nexusUpdateTask")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaskAPIApi#nexusUpdateTask")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the task | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusTask** | [**NexusTask**](NexusTask.md)| The details of the task | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

