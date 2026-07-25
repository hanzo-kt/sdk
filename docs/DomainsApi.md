# DomainsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**edgeCreateDomain**](DomainsApi.md#edgeCreateDomain) | **POST** /v1/edge/domains | Add custom domain |
| [**edgeDeleteDomain**](DomainsApi.md#edgeDeleteDomain) | **DELETE** /v1/edge/domains/{id} | Remove custom domain |
| [**edgeListDomains**](DomainsApi.md#edgeListDomains) | **GET** /v1/edge/domains | List custom domains |


<a id="edgeCreateDomain"></a>
# **edgeCreateDomain**
> EdgeDomain edgeCreateDomain(edgeDomainCreate)

Add custom domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainsApi()
val edgeDomainCreate : EdgeDomainCreate =  // EdgeDomainCreate | 
try {
    val result : EdgeDomain = apiInstance.edgeCreateDomain(edgeDomainCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainsApi#edgeCreateDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainsApi#edgeCreateDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeDomainCreate** | [**EdgeDomainCreate**](EdgeDomainCreate.md)|  | |

### Return type

[**EdgeDomain**](EdgeDomain.md)

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

<a id="edgeDeleteDomain"></a>
# **edgeDeleteDomain**
> kotlin.Any edgeDeleteDomain(id)

Remove custom domain

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.edgeDeleteDomain(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainsApi#edgeDeleteDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainsApi#edgeDeleteDomain")
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

<a id="edgeListDomains"></a>
# **edgeListDomains**
> kotlin.collections.List&lt;EdgeDomain&gt; edgeListDomains()

List custom domains

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DomainsApi()
try {
    val result : kotlin.collections.List<EdgeDomain> = apiInstance.edgeListDomains()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DomainsApi#edgeListDomains")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DomainsApi#edgeListDomains")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EdgeDomain&gt;**](EdgeDomain.md)

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

