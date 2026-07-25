# ClusterApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**paasAddClusterDomain**](ClusterApi.md#paasAddClusterDomain) | **POST** /v1/paas/cluster/domains | Add cluster domain |
| [**paasGetClusterInfo**](ClusterApi.md#paasGetClusterInfo) | **GET** /v1/paas/cluster/info | Get cluster info |
| [**paasGetSetupStatus**](ClusterApi.md#paasGetSetupStatus) | **GET** /v1/paas/cluster/setup-status | Check cluster setup status |
| [**paasListClusterDomains**](ClusterApi.md#paasListClusterDomains) | **GET** /v1/paas/cluster/domains | List cluster domains |
| [**paasRemoveClusterDomain**](ClusterApi.md#paasRemoveClusterDomain) | **DELETE** /v1/paas/cluster/domains/{domain} | Remove cluster domain |
| [**platformClusterGetNodes**](ClusterApi.md#platformClusterGetNodes) | **GET** /v1/platform/cluster/getNodes | List Docker Swarm nodes |


<a id="paasAddClusterDomain"></a>
# **paasAddClusterDomain**
> kotlin.Any paasAddClusterDomain(flowCreateCustomDomainRequest)

Add cluster domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
val flowCreateCustomDomainRequest : FlowCreateCustomDomainRequest =  // FlowCreateCustomDomainRequest | 
try {
    val result : kotlin.Any = apiInstance.paasAddClusterDomain(flowCreateCustomDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#paasAddClusterDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#paasAddClusterDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowCreateCustomDomainRequest** | [**FlowCreateCustomDomainRequest**](FlowCreateCustomDomainRequest.md)|  | |

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

<a id="paasGetClusterInfo"></a>
# **paasGetClusterInfo**
> PaasCluster paasGetClusterInfo()

Get cluster info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
try {
    val result : PaasCluster = apiInstance.paasGetClusterInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#paasGetClusterInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#paasGetClusterInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PaasCluster**](PaasCluster.md)

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

<a id="paasGetSetupStatus"></a>
# **paasGetSetupStatus**
> PaasGetSetupStatus200Response paasGetSetupStatus()

Check cluster setup status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
try {
    val result : PaasGetSetupStatus200Response = apiInstance.paasGetSetupStatus()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#paasGetSetupStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#paasGetSetupStatus")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PaasGetSetupStatus200Response**](PaasGetSetupStatus200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="paasListClusterDomains"></a>
# **paasListClusterDomains**
> kotlin.collections.List&lt;kotlin.String&gt; paasListClusterDomains()

List cluster domains

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.paasListClusterDomains()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#paasListClusterDomains")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#paasListClusterDomains")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

<a id="paasRemoveClusterDomain"></a>
# **paasRemoveClusterDomain**
> kotlin.Any paasRemoveClusterDomain(domain)

Remove cluster domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
val domain : kotlin.String = domain_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasRemoveClusterDomain(domain)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#paasRemoveClusterDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#paasRemoveClusterDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **domain** | **kotlin.String**|  | |

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

<a id="platformClusterGetNodes"></a>
# **platformClusterGetNodes**
> PlatformTRPCResult platformClusterGetNodes(input)

List Docker Swarm nodes

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ClusterApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformClusterGetNodes(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ClusterApi#platformClusterGetNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ClusterApi#platformClusterGetNodes")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

