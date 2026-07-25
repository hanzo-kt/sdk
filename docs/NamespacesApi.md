# NamespacesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kvCreateNamespace**](NamespacesApi.md#kvCreateNamespace) | **POST** /v1/kv/namespaces | Create namespace |
| [**kvDeleteNamespace**](NamespacesApi.md#kvDeleteNamespace) | **DELETE** /v1/kv/namespaces/{name} | Delete namespace and all keys |
| [**kvGetNamespace**](NamespacesApi.md#kvGetNamespace) | **GET** /v1/kv/namespaces/{name} | Get namespace |
| [**kvListNamespaces**](NamespacesApi.md#kvListNamespaces) | **GET** /v1/kv/namespaces | List namespaces |


<a id="kvCreateNamespace"></a>
# **kvCreateNamespace**
> KvNamespace kvCreateNamespace(kvCreateNamespaceRequest)

Create namespace

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NamespacesApi()
val kvCreateNamespaceRequest : KvCreateNamespaceRequest =  // KvCreateNamespaceRequest | 
try {
    val result : KvNamespace = apiInstance.kvCreateNamespace(kvCreateNamespaceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NamespacesApi#kvCreateNamespace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NamespacesApi#kvCreateNamespace")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kvCreateNamespaceRequest** | [**KvCreateNamespaceRequest**](KvCreateNamespaceRequest.md)|  | |

### Return type

[**KvNamespace**](KvNamespace.md)

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

<a id="kvDeleteNamespace"></a>
# **kvDeleteNamespace**
> kotlin.Any kvDeleteNamespace(name)

Delete namespace and all keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NamespacesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.kvDeleteNamespace(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NamespacesApi#kvDeleteNamespace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NamespacesApi#kvDeleteNamespace")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="kvGetNamespace"></a>
# **kvGetNamespace**
> KvNamespace kvGetNamespace(name)

Get namespace

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NamespacesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : KvNamespace = apiInstance.kvGetNamespace(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NamespacesApi#kvGetNamespace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NamespacesApi#kvGetNamespace")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**KvNamespace**](KvNamespace.md)

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

<a id="kvListNamespaces"></a>
# **kvListNamespaces**
> kotlin.collections.List&lt;KvNamespace&gt; kvListNamespaces()

List namespaces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NamespacesApi()
try {
    val result : kotlin.collections.List<KvNamespace> = apiInstance.kvListNamespaces()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NamespacesApi#kvListNamespaces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NamespacesApi#kvListNamespaces")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;KvNamespace&gt;**](KvNamespace.md)

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

