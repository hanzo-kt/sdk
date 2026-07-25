# ClustersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineDeleteCluster**](ClustersApi.md#engineDeleteCluster) | **DELETE** /v1/engine/clusters/{id} | Deregister cluster |
| [**engineGetCluster**](ClustersApi.md#engineGetCluster) | **GET** /v1/engine/clusters/{id} | Get cluster |
| [**engineListClusterNodes**](ClustersApi.md#engineListClusterNodes) | **GET** /v1/engine/clusters/{id}/nodes | List cluster nodes |
| [**engineListClusters**](ClustersApi.md#engineListClusters) | **GET** /v1/engine/clusters | List GPU clusters |
| [**engineRegisterCluster**](ClustersApi.md#engineRegisterCluster) | **POST** /v1/engine/clusters | Register GPU cluster |
| [**engineUpdateCluster**](ClustersApi.md#engineUpdateCluster) | **PUT** /v1/engine/clusters/{id} | Update cluster |
| [**kvCreateCluster**](ClustersApi.md#kvCreateCluster) | **POST** /v1/kv/clusters | Create KV cluster |
| [**kvDeleteCluster**](ClustersApi.md#kvDeleteCluster) | **DELETE** /v1/kv/clusters/{id} | Delete cluster |
| [**kvGetCluster**](ClustersApi.md#kvGetCluster) | **GET** /v1/kv/clusters/{id} | Get cluster |
| [**kvGetClusterStats**](ClustersApi.md#kvGetClusterStats) | **GET** /v1/kv/clusters/{id}/stats | Get cluster stats |
| [**kvListClusters**](ClustersApi.md#kvListClusters) | **GET** /v1/kv/clusters | List KV clusters |
| [**kvUpdateCluster**](ClustersApi.md#kvUpdateCluster) | **PUT** /v1/kv/clusters/{id} | Update cluster |
| [**visorCreatePool**](ClustersApi.md#visorCreatePool) | **POST** /v1/clusters/{clusterId}/pools | Add a node pool to a cluster |
| [**visorDeletePool**](ClustersApi.md#visorDeletePool) | **DELETE** /v1/clusters/{clusterId}/pools/{poolId} | Delete a node pool |
| [**visorListClusters**](ClustersApi.md#visorListClusters) | **GET** /v1/clusters | List DOKS clusters (projected from node pools) |
| [**visorScalePool**](ClustersApi.md#visorScalePool) | **POST** /v1/clusters/{clusterId}/pools/{poolId}/scale | Scale a node pool |


<a id="engineDeleteCluster"></a>
# **engineDeleteCluster**
> kotlin.Any engineDeleteCluster(id)

Deregister cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.engineDeleteCluster(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineDeleteCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineDeleteCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="engineGetCluster"></a>
# **engineGetCluster**
> EngineCluster engineGetCluster(id)

Get cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineCluster = apiInstance.engineGetCluster(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineGetCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineGetCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EngineCluster**](EngineCluster.md)

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

<a id="engineListClusterNodes"></a>
# **engineListClusterNodes**
> EngineListClusterNodes200Response engineListClusterNodes(id)

List cluster nodes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineListClusterNodes200Response = apiInstance.engineListClusterNodes(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineListClusterNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineListClusterNodes")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**EngineListClusterNodes200Response**](EngineListClusterNodes200Response.md)

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

<a id="engineListClusters"></a>
# **engineListClusters**
> EngineListClusters200Response engineListClusters(status, provider, page, pageSize)

List GPU clusters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val status : kotlin.String = status_example // kotlin.String | 
val provider : kotlin.String = provider_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EngineListClusters200Response = apiInstance.engineListClusters(status, provider, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineListClusters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineListClusters")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: online, offline, degraded, provisioning] |
| **provider** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**EngineListClusters200Response**](EngineListClusters200Response.md)

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

<a id="engineRegisterCluster"></a>
# **engineRegisterCluster**
> EngineCluster engineRegisterCluster(engineClusterCreate)

Register GPU cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val engineClusterCreate : EngineClusterCreate =  // EngineClusterCreate | 
try {
    val result : EngineCluster = apiInstance.engineRegisterCluster(engineClusterCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineRegisterCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineRegisterCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineClusterCreate** | [**EngineClusterCreate**](EngineClusterCreate.md)|  | |

### Return type

[**EngineCluster**](EngineCluster.md)

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

<a id="engineUpdateCluster"></a>
# **engineUpdateCluster**
> EngineCluster engineUpdateCluster(id, engineUpdateClusterRequest)

Update cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val engineUpdateClusterRequest : EngineUpdateClusterRequest =  // EngineUpdateClusterRequest | 
try {
    val result : EngineCluster = apiInstance.engineUpdateCluster(id, engineUpdateClusterRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#engineUpdateCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#engineUpdateCluster")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineUpdateClusterRequest** | [**EngineUpdateClusterRequest**](EngineUpdateClusterRequest.md)|  | |

### Return type

[**EngineCluster**](EngineCluster.md)

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

<a id="kvCreateCluster"></a>
# **kvCreateCluster**
> KvCluster kvCreateCluster(kvClusterCreate)

Create KV cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val kvClusterCreate : KvClusterCreate =  // KvClusterCreate | 
try {
    val result : KvCluster = apiInstance.kvCreateCluster(kvClusterCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvCreateCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvCreateCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvClusterCreate** | [**KvClusterCreate**](KvClusterCreate.md)|  | |

### Return type

[**KvCluster**](KvCluster.md)

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

<a id="kvDeleteCluster"></a>
# **kvDeleteCluster**
> kotlin.Any kvDeleteCluster(id)

Delete cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kvDeleteCluster(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvDeleteCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvDeleteCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="kvGetCluster"></a>
# **kvGetCluster**
> KvCluster kvGetCluster(id)

Get cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KvCluster = apiInstance.kvGetCluster(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvGetCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvGetCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**KvCluster**](KvCluster.md)

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

<a id="kvGetClusterStats"></a>
# **kvGetClusterStats**
> KvGetClusterStats200Response kvGetClusterStats(id)

Get cluster stats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KvGetClusterStats200Response = apiInstance.kvGetClusterStats(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvGetClusterStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvGetClusterStats")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**KvGetClusterStats200Response**](KvGetClusterStats200Response.md)

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

<a id="kvListClusters"></a>
# **kvListClusters**
> KvListClusters200Response kvListClusters(status)

List KV clusters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val status : kotlin.String = status_example // kotlin.String | 
try {
    val result : KvListClusters200Response = apiInstance.kvListClusters(status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvListClusters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvListClusters")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] [enum: provisioning, running, degraded, stopped] |

### Return type

[**KvListClusters200Response**](KvListClusters200Response.md)

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

<a id="kvUpdateCluster"></a>
# **kvUpdateCluster**
> KvCluster kvUpdateCluster(id, kvUpdateClusterRequest)

Update cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kvUpdateClusterRequest : KvUpdateClusterRequest =  // KvUpdateClusterRequest | 
try {
    val result : KvCluster = apiInstance.kvUpdateCluster(id, kvUpdateClusterRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#kvUpdateCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#kvUpdateCluster")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvUpdateClusterRequest** | [**KvUpdateClusterRequest**](KvUpdateClusterRequest.md)|  | |

### Return type

[**KvCluster**](KvCluster.md)

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

<a id="visorCreatePool"></a>
# **visorCreatePool**
> VisorNodePoolView visorCreatePool(clusterId, visorPoolRequest)

Add a node pool to a cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val clusterId : kotlin.String = clusterId_example // kotlin.String | 
val visorPoolRequest : VisorPoolRequest =  // VisorPoolRequest | 
try {
    val result : VisorNodePoolView = apiInstance.visorCreatePool(clusterId, visorPoolRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#visorCreatePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#visorCreatePool")
    e.printStackTrace()
}
```

### Parameters
| **clusterId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visorPoolRequest** | [**VisorPoolRequest**](VisorPoolRequest.md)|  | |

### Return type

[**VisorNodePoolView**](VisorNodePoolView.md)

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

<a id="visorDeletePool"></a>
# **visorDeletePool**
> visorDeletePool(clusterId, poolId, provider)

Delete a node pool

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val clusterId : kotlin.String = clusterId_example // kotlin.String | 
val poolId : kotlin.String = poolId_example // kotlin.String | 
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    apiInstance.visorDeletePool(clusterId, poolId, provider)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#visorDeletePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#visorDeletePool")
    e.printStackTrace()
}
```

### Parameters
| **clusterId** | **kotlin.String**|  | |
| **poolId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | |

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
 - **Accept**: application/json

<a id="visorListClusters"></a>
# **visorListClusters**
> VisorListClusters200Response visorListClusters()

List DOKS clusters (projected from node pools)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
try {
    val result : VisorListClusters200Response = apiInstance.visorListClusters()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#visorListClusters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#visorListClusters")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListClusters200Response**](VisorListClusters200Response.md)

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

<a id="visorScalePool"></a>
# **visorScalePool**
> VisorNodePoolView visorScalePool(clusterId, poolId, visorScaleRequest)

Scale a node pool

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClustersApi()
val clusterId : kotlin.String = clusterId_example // kotlin.String | 
val poolId : kotlin.String = poolId_example // kotlin.String | 
val visorScaleRequest : VisorScaleRequest =  // VisorScaleRequest | 
try {
    val result : VisorNodePoolView = apiInstance.visorScalePool(clusterId, poolId, visorScaleRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClustersApi#visorScalePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClustersApi#visorScalePool")
    e.printStackTrace()
}
```

### Parameters
| **clusterId** | **kotlin.String**|  | |
| **poolId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visorScaleRequest** | [**VisorScaleRequest**](VisorScaleRequest.md)|  | |

### Return type

[**VisorNodePoolView**](VisorNodePoolView.md)

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

