# DatastoreApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**provisioningCreateDatastore**](DatastoreApi.md#provisioningCreateDatastore) | **POST** /v1/datastore | Provision a datastore resource (dedicated per-org instance) |
| [**provisioningDeleteDatastore**](DatastoreApi.md#provisioningDeleteDatastore) | **DELETE** /v1/datastore/{name} | Deprovision a datastore instance |
| [**provisioningGetDatastore**](DatastoreApi.md#provisioningGetDatastore) | **GET** /v1/datastore/{name} | Get one datastore resource (reconciles live instance status) |
| [**provisioningListDatastore**](DatastoreApi.md#provisioningListDatastore) | **GET** /v1/datastore | List datastore resources for the caller&#39;s org |


<a id="provisioningCreateDatastore"></a>
# **provisioningCreateDatastore**
> ProvisioningCreateResponse provisioningCreateDatastore(provisioningCreateRequest)

Provision a datastore resource (dedicated per-org instance)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatastoreApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateDatastore(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatastoreApi#provisioningCreateDatastore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatastoreApi#provisioningCreateDatastore")
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

<a id="provisioningDeleteDatastore"></a>
# **provisioningDeleteDatastore**
> provisioningDeleteDatastore(name)

Deprovision a datastore instance

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatastoreApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteDatastore(name)
} catch (e: ClientException) {
    println("4xx response calling DatastoreApi#provisioningDeleteDatastore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatastoreApi#provisioningDeleteDatastore")
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

<a id="provisioningGetDatastore"></a>
# **provisioningGetDatastore**
> ProvisioningGetResponse provisioningGetDatastore(name)

Get one datastore resource (reconciles live instance status)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatastoreApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetDatastore(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatastoreApi#provisioningGetDatastore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatastoreApi#provisioningGetDatastore")
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

<a id="provisioningListDatastore"></a>
# **provisioningListDatastore**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListDatastore()

List datastore resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatastoreApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListDatastore()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatastoreApi#provisioningListDatastore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatastoreApi#provisioningListDatastore")
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

