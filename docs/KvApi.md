# KvApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**provisioningCreateKv**](KvApi.md#provisioningCreateKv) | **POST** /v1/kv | Provision a key-value resource |
| [**provisioningDeleteKv**](KvApi.md#provisioningDeleteKv) | **DELETE** /v1/kv/{name} | Deprovision a key-value resource |
| [**provisioningGetKv**](KvApi.md#provisioningGetKv) | **GET** /v1/kv/{name} | Get one key-value resource |
| [**provisioningListKv**](KvApi.md#provisioningListKv) | **GET** /v1/kv | List key-value resources for the caller&#39;s org |


<a id="provisioningCreateKv"></a>
# **provisioningCreateKv**
> ProvisioningCreateResponse provisioningCreateKv(provisioningCreateRequest)

Provision a key-value resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KvApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateKv(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KvApi#provisioningCreateKv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KvApi#provisioningCreateKv")
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

<a id="provisioningDeleteKv"></a>
# **provisioningDeleteKv**
> provisioningDeleteKv(name)

Deprovision a key-value resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KvApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteKv(name)
} catch (e: ClientException) {
    println("4xx response calling KvApi#provisioningDeleteKv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KvApi#provisioningDeleteKv")
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

<a id="provisioningGetKv"></a>
# **provisioningGetKv**
> ProvisioningGetResponse provisioningGetKv(name)

Get one key-value resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KvApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetKv(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KvApi#provisioningGetKv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KvApi#provisioningGetKv")
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

<a id="provisioningListKv"></a>
# **provisioningListKv**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListKv()

List key-value resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KvApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListKv()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KvApi#provisioningListKv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KvApi#provisioningListKv")
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

