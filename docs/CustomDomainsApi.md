# CustomDomainsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowCreateCustomDomain**](CustomDomainsApi.md#flowCreateCustomDomain) | **POST** /v1/flow/custom-domains | Add a custom domain (EE) |
| [**flowDeleteCustomDomain**](CustomDomainsApi.md#flowDeleteCustomDomain) | **DELETE** /v1/flow/custom-domains/{id} | Remove a custom domain (EE) |
| [**flowListCustomDomains**](CustomDomainsApi.md#flowListCustomDomains) | **GET** /v1/flow/custom-domains | List custom domains (EE) |


<a id="flowCreateCustomDomain"></a>
# **flowCreateCustomDomain**
> kotlin.Any flowCreateCustomDomain(flowCreateCustomDomainRequest)

Add a custom domain (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomDomainsApi()
val flowCreateCustomDomainRequest : FlowCreateCustomDomainRequest =  // FlowCreateCustomDomainRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateCustomDomain(flowCreateCustomDomainRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomDomainsApi#flowCreateCustomDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomDomainsApi#flowCreateCustomDomain")
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

<a id="flowDeleteCustomDomain"></a>
# **flowDeleteCustomDomain**
> flowDeleteCustomDomain(id)

Remove a custom domain (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomDomainsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteCustomDomain(id)
} catch (e: ClientException) {
    println("4xx response calling CustomDomainsApi#flowDeleteCustomDomain")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomDomainsApi#flowDeleteCustomDomain")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowListCustomDomains"></a>
# **flowListCustomDomains**
> kotlin.Any flowListCustomDomains()

List custom domains (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomDomainsApi()
try {
    val result : kotlin.Any = apiInstance.flowListCustomDomains()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomDomainsApi#flowListCustomDomains")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomDomainsApi#flowListCustomDomains")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

