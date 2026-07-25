# ContainersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**paasCreateContainer**](ContainersApi.md#paasCreateContainer) | **POST** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers | Create container |
| [**paasDeleteContainer**](ContainersApi.md#paasDeleteContainer) | **DELETE** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId} | Delete container |
| [**paasDeployContainer**](ContainersApi.md#paasDeployContainer) | **POST** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId}/deploy | Trigger deployment (Nixpacks build + deploy) |
| [**paasGetContainer**](ContainersApi.md#paasGetContainer) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId} | Get container |
| [**paasListContainerPods**](ContainersApi.md#paasListContainerPods) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId}/pods | List container pods |
| [**paasListContainers**](ContainersApi.md#paasListContainers) | **GET** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers | List containers |
| [**paasUpdateContainer**](ContainersApi.md#paasUpdateContainer) | **PUT** /v1/paas/org/{orgId}/project/{projectId}/env/{envId}/containers/{containerId} | Update container |


<a id="paasCreateContainer"></a>
# **paasCreateContainer**
> PaasContainer paasCreateContainer(orgId, projectId, envId, paasCreateContainerRequest)

Create container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val paasCreateContainerRequest : PaasCreateContainerRequest =  // PaasCreateContainerRequest | 
try {
    val result : PaasContainer = apiInstance.paasCreateContainer(orgId, projectId, envId, paasCreateContainerRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasCreateContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasCreateContainer")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasCreateContainerRequest** | [**PaasCreateContainerRequest**](PaasCreateContainerRequest.md)|  | |

### Return type

[**PaasContainer**](PaasContainer.md)

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

<a id="paasDeleteContainer"></a>
# **paasDeleteContainer**
> kotlin.Any paasDeleteContainer(orgId, projectId, envId, containerId)

Delete container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeleteContainer(orgId, projectId, envId, containerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasDeleteContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasDeleteContainer")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **containerId** | **kotlin.String**|  | |

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

<a id="paasDeployContainer"></a>
# **paasDeployContainer**
> kotlin.Any paasDeployContainer(orgId, projectId, envId, containerId)

Trigger deployment (Nixpacks build + deploy)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeployContainer(orgId, projectId, envId, containerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasDeployContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasDeployContainer")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **containerId** | **kotlin.String**|  | |

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

<a id="paasGetContainer"></a>
# **paasGetContainer**
> PaasContainer paasGetContainer(orgId, projectId, envId, containerId)

Get container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
try {
    val result : PaasContainer = apiInstance.paasGetContainer(orgId, projectId, envId, containerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasGetContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasGetContainer")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **containerId** | **kotlin.String**|  | |

### Return type

[**PaasContainer**](PaasContainer.md)

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

<a id="paasListContainerPods"></a>
# **paasListContainerPods**
> kotlin.collections.List&lt;PaasListContainerPods200ResponseInner&gt; paasListContainerPods(orgId, projectId, envId, containerId)

List container pods

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaasListContainerPods200ResponseInner> = apiInstance.paasListContainerPods(orgId, projectId, envId, containerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasListContainerPods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasListContainerPods")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **containerId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PaasListContainerPods200ResponseInner&gt;**](PaasListContainerPods200ResponseInner.md)

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

<a id="paasListContainers"></a>
# **paasListContainers**
> kotlin.collections.List&lt;PaasContainer&gt; paasListContainers(orgId, projectId, envId)

List containers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaasContainer> = apiInstance.paasListContainers(orgId, projectId, envId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasListContainers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasListContainers")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **envId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PaasContainer&gt;**](PaasContainer.md)

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

<a id="paasUpdateContainer"></a>
# **paasUpdateContainer**
> kotlin.Any paasUpdateContainer(orgId, projectId, envId, containerId, body)

Update container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainersApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val envId : kotlin.String = envId_example // kotlin.String | 
val containerId : kotlin.String = containerId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.paasUpdateContainer(orgId, projectId, envId, containerId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainersApi#paasUpdateContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainersApi#paasUpdateContainer")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| **envId** | **kotlin.String**|  | |
| **containerId** | **kotlin.String**|  | |
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

