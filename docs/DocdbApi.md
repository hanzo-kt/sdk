# DocdbApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**provisioningCreateDocdb**](DocdbApi.md#provisioningCreateDocdb) | **POST** /v1/docdb | Provision a document-database resource (dedicated per-org instance) |
| [**provisioningDeleteDocdb**](DocdbApi.md#provisioningDeleteDocdb) | **DELETE** /v1/docdb/{name} | Deprovision a document-database instance |
| [**provisioningGetDocdb**](DocdbApi.md#provisioningGetDocdb) | **GET** /v1/docdb/{name} | Get one document-database resource (reconciles live instance status) |
| [**provisioningListDocdb**](DocdbApi.md#provisioningListDocdb) | **GET** /v1/docdb | List document-database resources for the caller&#39;s org |


<a id="provisioningCreateDocdb"></a>
# **provisioningCreateDocdb**
> ProvisioningCreateResponse provisioningCreateDocdb(provisioningCreateRequest)

Provision a document-database resource (dedicated per-org instance)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocdbApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateDocdb(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocdbApi#provisioningCreateDocdb")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocdbApi#provisioningCreateDocdb")
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

<a id="provisioningDeleteDocdb"></a>
# **provisioningDeleteDocdb**
> provisioningDeleteDocdb(name)

Deprovision a document-database instance

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocdbApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteDocdb(name)
} catch (e: ClientException) {
    println("4xx response calling DocdbApi#provisioningDeleteDocdb")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocdbApi#provisioningDeleteDocdb")
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

<a id="provisioningGetDocdb"></a>
# **provisioningGetDocdb**
> ProvisioningGetResponse provisioningGetDocdb(name)

Get one document-database resource (reconciles live instance status)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocdbApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetDocdb(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocdbApi#provisioningGetDocdb")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocdbApi#provisioningGetDocdb")
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

<a id="provisioningListDocdb"></a>
# **provisioningListDocdb**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListDocdb()

List document-database resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocdbApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListDocdb()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocdbApi#provisioningListDocdb")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocdbApi#provisioningListDocdb")
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

