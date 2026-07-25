# VectorApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**productGetVectorStats**](VectorApi.md#productGetVectorStats) | **GET** /v1/vector/stats | Get aggregate vector statistics |
| [**provisioningCreateVector**](VectorApi.md#provisioningCreateVector) | **POST** /v1/vector | Provision a vector resource |
| [**provisioningDeleteVector**](VectorApi.md#provisioningDeleteVector) | **DELETE** /v1/vector/{name} | Deprovision a vector resource |
| [**provisioningGetVector**](VectorApi.md#provisioningGetVector) | **GET** /v1/vector/{name} | Get one vector resource |
| [**provisioningListVector**](VectorApi.md#provisioningListVector) | **GET** /v1/vector | List vector resources for the caller&#39;s org |


<a id="productGetVectorStats"></a>
# **productGetVectorStats**
> ProductVectorStats productGetVectorStats()

Get aggregate vector statistics

Returns totals aggregated across all Qdrant collections: collection count, vector count, and storage bytes. If the upstream is unreachable, returns HTTP 200 with all counters zeroed. Authenticated with the opaque vector service key. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorApi()
try {
    val result : ProductVectorStats = apiInstance.productGetVectorStats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorApi#productGetVectorStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorApi#productGetVectorStats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ProductVectorStats**](ProductVectorStats.md)

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

<a id="provisioningCreateVector"></a>
# **provisioningCreateVector**
> ProvisioningCreateResponse provisioningCreateVector(provisioningCreateRequest)

Provision a vector resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateVector(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorApi#provisioningCreateVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorApi#provisioningCreateVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provisioningCreateRequest** | [**ProvisioningCreateRequest**](ProvisioningCreateRequest.md)|  | |

### Return type

[**ProvisioningCreateResponse**](ProvisioningCreateResponse.md)

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

<a id="provisioningDeleteVector"></a>
# **provisioningDeleteVector**
> provisioningDeleteVector(name)

Deprovision a vector resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteVector(name)
} catch (e: ClientException) {
    println("4xx response calling VectorApi#provisioningDeleteVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorApi#provisioningDeleteVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The user-supplied resource name (slug). Lowercased and trimmed server-side; must match &#x60;^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$&#x60;.  | |

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

<a id="provisioningGetVector"></a>
# **provisioningGetVector**
> ProvisioningGetResponse provisioningGetVector(name)

Get one vector resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetVector(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorApi#provisioningGetVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorApi#provisioningGetVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The user-supplied resource name (slug). Lowercased and trimmed server-side; must match &#x60;^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$&#x60;.  | |

### Return type

[**ProvisioningGetResponse**](ProvisioningGetResponse.md)

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

<a id="provisioningListVector"></a>
# **provisioningListVector**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListVector()

List vector resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListVector()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorApi#provisioningListVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorApi#provisioningListVector")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProvisioningListItem&gt;**](ProvisioningListItem.md)

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

