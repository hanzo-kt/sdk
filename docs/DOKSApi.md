# DOKSApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**paasAddDOKSNodePool**](DOKSApi.md#paasAddDOKSNodePool) | **POST** /v1/paas/cluster/doks/{orgId}/node-pools | Add node pool |
| [**paasDeleteDOKSNodePool**](DOKSApi.md#paasDeleteDOKSNodePool) | **DELETE** /v1/paas/cluster/doks/{orgId}/node-pools/{poolId} | Delete node pool |
| [**paasDestroyDOKS**](DOKSApi.md#paasDestroyDOKS) | **DELETE** /v1/paas/cluster/doks/{orgId} | Destroy DOKS cluster |
| [**paasGetDOKSFleet**](DOKSApi.md#paasGetDOKSFleet) | **GET** /v1/paas/cluster/doks/fleet | Fleet overview (all org clusters) |
| [**paasGetDOKSKubeconfig**](DOKSApi.md#paasGetDOKSKubeconfig) | **GET** /v1/paas/cluster/doks/{orgId}/kubeconfig | Download kubeconfig |
| [**paasGetDOKSOptions**](DOKSApi.md#paasGetDOKSOptions) | **GET** /v1/paas/cluster/doks/options | Available regions and node sizes |
| [**paasGetDOKSPricing**](DOKSApi.md#paasGetDOKSPricing) | **GET** /v1/paas/cluster/doks/pricing/{sizeSlug} | Get droplet pricing |
| [**paasGetDOKSStatus**](DOKSApi.md#paasGetDOKSStatus) | **GET** /v1/paas/cluster/doks/{orgId}/status | Get cluster status (polls DO API) |
| [**paasListDOKSNodePools**](DOKSApi.md#paasListDOKSNodePools) | **GET** /v1/paas/cluster/doks/{orgId}/node-pools | List node pools |
| [**paasProvisionDOKS**](DOKSApi.md#paasProvisionDOKS) | **POST** /v1/paas/cluster/doks/provision | Provision new DOKS cluster for org |
| [**paasUpdateDOKSNodePool**](DOKSApi.md#paasUpdateDOKSNodePool) | **PUT** /v1/paas/cluster/doks/{orgId}/node-pools/{poolId} | Update node pool |
| [**paasUpgradeDOKSHA**](DOKSApi.md#paasUpgradeDOKSHA) | **POST** /v1/paas/cluster/doks/{orgId}/upgrade-ha | Upgrade to HA control plane |


<a id="paasAddDOKSNodePool"></a>
# **paasAddDOKSNodePool**
> kotlin.Any paasAddDOKSNodePool(orgId, paasNodePool)

Add node pool

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val paasNodePool : PaasNodePool =  // PaasNodePool | 
try {
    val result : kotlin.Any = apiInstance.paasAddDOKSNodePool(orgId, paasNodePool)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasAddDOKSNodePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasAddDOKSNodePool")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasNodePool** | [**PaasNodePool**](PaasNodePool.md)|  | |

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

<a id="paasDeleteDOKSNodePool"></a>
# **paasDeleteDOKSNodePool**
> kotlin.Any paasDeleteDOKSNodePool(orgId, poolId)

Delete node pool

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val poolId : kotlin.String = poolId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeleteDOKSNodePool(orgId, poolId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasDeleteDOKSNodePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasDeleteDOKSNodePool")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **poolId** | **kotlin.String**|  | |

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

<a id="paasDestroyDOKS"></a>
# **paasDestroyDOKS**
> kotlin.Any paasDestroyDOKS(orgId, confirm)

Destroy DOKS cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val confirm : kotlin.Boolean = true // kotlin.Boolean | Must be true to confirm destruction
try {
    val result : kotlin.Any = apiInstance.paasDestroyDOKS(orgId, confirm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasDestroyDOKS")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasDestroyDOKS")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirm** | **kotlin.Boolean**| Must be true to confirm destruction | |

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

<a id="paasGetDOKSFleet"></a>
# **paasGetDOKSFleet**
> PaasFleetOverview paasGetDOKSFleet()

Fleet overview (all org clusters)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
try {
    val result : PaasFleetOverview = apiInstance.paasGetDOKSFleet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasGetDOKSFleet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasGetDOKSFleet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PaasFleetOverview**](PaasFleetOverview.md)

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

<a id="paasGetDOKSKubeconfig"></a>
# **paasGetDOKSKubeconfig**
> kotlin.String paasGetDOKSKubeconfig(orgId)

Download kubeconfig

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.paasGetDOKSKubeconfig(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasGetDOKSKubeconfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasGetDOKSKubeconfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

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

<a id="paasGetDOKSOptions"></a>
# **paasGetDOKSOptions**
> PaasGetDOKSOptions200Response paasGetDOKSOptions()

Available regions and node sizes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
try {
    val result : PaasGetDOKSOptions200Response = apiInstance.paasGetDOKSOptions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasGetDOKSOptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasGetDOKSOptions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PaasGetDOKSOptions200Response**](PaasGetDOKSOptions200Response.md)

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

<a id="paasGetDOKSPricing"></a>
# **paasGetDOKSPricing**
> PaasGetDOKSPricing200Response paasGetDOKSPricing(sizeSlug)

Get droplet pricing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val sizeSlug : kotlin.String = sizeSlug_example // kotlin.String | 
try {
    val result : PaasGetDOKSPricing200Response = apiInstance.paasGetDOKSPricing(sizeSlug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasGetDOKSPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasGetDOKSPricing")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sizeSlug** | **kotlin.String**|  | |

### Return type

[**PaasGetDOKSPricing200Response**](PaasGetDOKSPricing200Response.md)

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

<a id="paasGetDOKSStatus"></a>
# **paasGetDOKSStatus**
> PaasDOKSCluster paasGetDOKSStatus(orgId)

Get cluster status (polls DO API)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : PaasDOKSCluster = apiInstance.paasGetDOKSStatus(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasGetDOKSStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasGetDOKSStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

### Return type

[**PaasDOKSCluster**](PaasDOKSCluster.md)

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

<a id="paasListDOKSNodePools"></a>
# **paasListDOKSNodePools**
> kotlin.collections.List&lt;PaasNodePool&gt; paasListDOKSNodePools(orgId)

List node pools

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaasNodePool> = apiInstance.paasListDOKSNodePools(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasListDOKSNodePools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasListDOKSNodePools")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PaasNodePool&gt;**](PaasNodePool.md)

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

<a id="paasProvisionDOKS"></a>
# **paasProvisionDOKS**
> PaasDOKSCluster paasProvisionDOKS(paasProvisionDOKSRequest)

Provision new DOKS cluster for org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val paasProvisionDOKSRequest : PaasProvisionDOKSRequest =  // PaasProvisionDOKSRequest | 
try {
    val result : PaasDOKSCluster = apiInstance.paasProvisionDOKS(paasProvisionDOKSRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasProvisionDOKS")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasProvisionDOKS")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasProvisionDOKSRequest** | [**PaasProvisionDOKSRequest**](PaasProvisionDOKSRequest.md)|  | |

### Return type

[**PaasDOKSCluster**](PaasDOKSCluster.md)

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

<a id="paasUpdateDOKSNodePool"></a>
# **paasUpdateDOKSNodePool**
> kotlin.Any paasUpdateDOKSNodePool(orgId, poolId, paasUpdateDOKSNodePoolRequest)

Update node pool

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val poolId : kotlin.String = poolId_example // kotlin.String | 
val paasUpdateDOKSNodePoolRequest : PaasUpdateDOKSNodePoolRequest =  // PaasUpdateDOKSNodePoolRequest | 
try {
    val result : kotlin.Any = apiInstance.paasUpdateDOKSNodePool(orgId, poolId, paasUpdateDOKSNodePoolRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasUpdateDOKSNodePool")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasUpdateDOKSNodePool")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **poolId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasUpdateDOKSNodePoolRequest** | [**PaasUpdateDOKSNodePoolRequest**](PaasUpdateDOKSNodePoolRequest.md)|  | |

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

<a id="paasUpgradeDOKSHA"></a>
# **paasUpgradeDOKSHA**
> kotlin.Any paasUpgradeDOKSHA(orgId)

Upgrade to HA control plane

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DOKSApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasUpgradeDOKSHA(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DOKSApi#paasUpgradeDOKSHA")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DOKSApi#paasUpgradeDOKSHA")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

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

