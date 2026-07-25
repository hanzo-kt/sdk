# WorkflowAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddWorkflow**](WorkflowAPIApi.md#cloudApiControllerAddWorkflow) | **POST** /v1/cloud/add-workflow | Api Controller Add Workflow |
| [**cloudApiControllerDeleteWorkflow**](WorkflowAPIApi.md#cloudApiControllerDeleteWorkflow) | **POST** /v1/cloud/delete-workflow | Api Controller Delete Workflow |
| [**cloudApiControllerGetGlobalWorkflows**](WorkflowAPIApi.md#cloudApiControllerGetGlobalWorkflows) | **GET** /v1/cloud/get-global-workflows | Api Controller Get Global Workflows |
| [**cloudApiControllerGetWorkflow**](WorkflowAPIApi.md#cloudApiControllerGetWorkflow) | **GET** /v1/cloud/get-workflow | Api Controller Get Workflow |
| [**cloudApiControllerGetWorkflows**](WorkflowAPIApi.md#cloudApiControllerGetWorkflows) | **GET** /v1/cloud/get-workflows | Api Controller Get Workflows |
| [**cloudApiControllerUpdateWorkflow**](WorkflowAPIApi.md#cloudApiControllerUpdateWorkflow) | **POST** /v1/cloud/update-workflow | Api Controller Update Workflow |
| [**nexusAddWorkflow**](WorkflowAPIApi.md#nexusAddWorkflow) | **POST** /v1/nexus/add-workflow | add Workflow |
| [**nexusDeleteWorkflow**](WorkflowAPIApi.md#nexusDeleteWorkflow) | **POST** /v1/nexus/delete-workflow | delete Workflow |
| [**nexusGetGlobalWorkflows**](WorkflowAPIApi.md#nexusGetGlobalWorkflows) | **GET** /v1/nexus/get-global-workflows | get Global Workflows |
| [**nexusGetWorkflow**](WorkflowAPIApi.md#nexusGetWorkflow) | **GET** /v1/nexus/get-workflow | get Workflow |
| [**nexusGetWorkflows**](WorkflowAPIApi.md#nexusGetWorkflows) | **GET** /v1/nexus/get-workflows | get Workflows |
| [**nexusUpdateWorkflow**](WorkflowAPIApi.md#nexusUpdateWorkflow) | **POST** /v1/nexus/update-workflow | update Workflow |


<a id="cloudApiControllerAddWorkflow"></a>
# **cloudApiControllerAddWorkflow**
> CloudControllersResponse cloudApiControllerAddWorkflow(cloudObjectWorkflow)

Api Controller Add Workflow

add workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddWorkflow(cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerAddWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerAddWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

<a id="cloudApiControllerDeleteWorkflow"></a>
# **cloudApiControllerDeleteWorkflow**
> CloudControllersResponse cloudApiControllerDeleteWorkflow(cloudObjectWorkflow)

Api Controller Delete Workflow

delete workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteWorkflow(cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerDeleteWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerDeleteWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

<a id="cloudApiControllerGetGlobalWorkflows"></a>
# **cloudApiControllerGetGlobalWorkflows**
> kotlin.collections.List&lt;CloudObjectWorkflow&gt; cloudApiControllerGetGlobalWorkflows()

Api Controller Get Global Workflows

get global workflows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectWorkflow> = apiInstance.cloudApiControllerGetGlobalWorkflows()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerGetGlobalWorkflows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerGetGlobalWorkflows")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectWorkflow&gt;**](CloudObjectWorkflow.md)

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

<a id="cloudApiControllerGetWorkflow"></a>
# **cloudApiControllerGetWorkflow**
> CloudObjectWorkflow cloudApiControllerGetWorkflow(id)

Api Controller Get Workflow

get workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of workflow
try {
    val result : CloudObjectWorkflow = apiInstance.cloudApiControllerGetWorkflow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerGetWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerGetWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of workflow | |

### Return type

[**CloudObjectWorkflow**](CloudObjectWorkflow.md)

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

<a id="cloudApiControllerGetWorkflows"></a>
# **cloudApiControllerGetWorkflows**
> kotlin.collections.List&lt;CloudObjectWorkflow&gt; cloudApiControllerGetWorkflows(owner)

Api Controller Get Workflows

get workflows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of workflow
try {
    val result : kotlin.collections.List<CloudObjectWorkflow> = apiInstance.cloudApiControllerGetWorkflows(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerGetWorkflows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerGetWorkflows")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of workflow | |

### Return type

[**kotlin.collections.List&lt;CloudObjectWorkflow&gt;**](CloudObjectWorkflow.md)

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

<a id="cloudApiControllerUpdateWorkflow"></a>
# **cloudApiControllerUpdateWorkflow**
> CloudControllersResponse cloudApiControllerUpdateWorkflow(id, cloudObjectWorkflow)

Api Controller Update Workflow

update workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the workflow
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateWorkflow(id, cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#cloudApiControllerUpdateWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#cloudApiControllerUpdateWorkflow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the workflow | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

<a id="nexusAddWorkflow"></a>
# **nexusAddWorkflow**
> NexusResponse nexusAddWorkflow(cloudObjectWorkflow)

add Workflow

Add a workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : NexusResponse = apiInstance.nexusAddWorkflow(cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusAddWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusAddWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

<a id="nexusDeleteWorkflow"></a>
# **nexusDeleteWorkflow**
> NexusResponse nexusDeleteWorkflow(cloudObjectWorkflow)

delete Workflow

Delete a workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : NexusResponse = apiInstance.nexusDeleteWorkflow(cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusDeleteWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusDeleteWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

<a id="nexusGetGlobalWorkflows"></a>
# **nexusGetGlobalWorkflows**
> kotlin.collections.List&lt;CloudObjectWorkflow&gt; nexusGetGlobalWorkflows()

get Global Workflows

Get global workflows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectWorkflow> = apiInstance.nexusGetGlobalWorkflows()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusGetGlobalWorkflows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusGetGlobalWorkflows")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectWorkflow&gt;**](CloudObjectWorkflow.md)

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

<a id="nexusGetWorkflow"></a>
# **nexusGetWorkflow**
> CloudObjectWorkflow nexusGetWorkflow(id)

get Workflow

Get a workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the workflow
try {
    val result : CloudObjectWorkflow = apiInstance.nexusGetWorkflow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusGetWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusGetWorkflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the workflow | |

### Return type

[**CloudObjectWorkflow**](CloudObjectWorkflow.md)

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

<a id="nexusGetWorkflows"></a>
# **nexusGetWorkflows**
> kotlin.collections.List&lt;CloudObjectWorkflow&gt; nexusGetWorkflows(owner)

get Workflows

Get workflows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the workflows
try {
    val result : kotlin.collections.List<CloudObjectWorkflow> = apiInstance.nexusGetWorkflows(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusGetWorkflows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusGetWorkflows")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the workflows | |

### Return type

[**kotlin.collections.List&lt;CloudObjectWorkflow&gt;**](CloudObjectWorkflow.md)

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

<a id="nexusUpdateWorkflow"></a>
# **nexusUpdateWorkflow**
> NexusResponse nexusUpdateWorkflow(id, cloudObjectWorkflow)

update Workflow

Update a workflow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WorkflowAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the workflow
val cloudObjectWorkflow : CloudObjectWorkflow =  // CloudObjectWorkflow | The details of the workflow
try {
    val result : NexusResponse = apiInstance.nexusUpdateWorkflow(id, cloudObjectWorkflow)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowAPIApi#nexusUpdateWorkflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowAPIApi#nexusUpdateWorkflow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the workflow | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectWorkflow** | [**CloudObjectWorkflow**](CloudObjectWorkflow.md)| The details of the workflow | |

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

