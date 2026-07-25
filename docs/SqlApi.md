# SqlApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**provisioningCreateSql**](SqlApi.md#provisioningCreateSql) | **POST** /v1/sql | Provision a SQL resource |
| [**provisioningDeleteSql**](SqlApi.md#provisioningDeleteSql) | **DELETE** /v1/sql/{name} | Deprovision a SQL resource |
| [**provisioningGetSql**](SqlApi.md#provisioningGetSql) | **GET** /v1/sql/{name} | Get one SQL resource |
| [**provisioningListSql**](SqlApi.md#provisioningListSql) | **GET** /v1/sql | List SQL resources for the caller&#39;s org |


<a id="provisioningCreateSql"></a>
# **provisioningCreateSql**
> ProvisioningCreateResponse provisioningCreateSql(provisioningCreateRequest)

Provision a SQL resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SqlApi()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateSql(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SqlApi#provisioningCreateSql")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SqlApi#provisioningCreateSql")
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

<a id="provisioningDeleteSql"></a>
# **provisioningDeleteSql**
> provisioningDeleteSql(name)

Deprovision a SQL resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SqlApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteSql(name)
} catch (e: ClientException) {
    println("4xx response calling SqlApi#provisioningDeleteSql")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SqlApi#provisioningDeleteSql")
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

<a id="provisioningGetSql"></a>
# **provisioningGetSql**
> ProvisioningGetResponse provisioningGetSql(name)

Get one SQL resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SqlApi()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetSql(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SqlApi#provisioningGetSql")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SqlApi#provisioningGetSql")
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

<a id="provisioningListSql"></a>
# **provisioningListSql**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListSql()

List SQL resources for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SqlApi()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListSql()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SqlApi#provisioningListSql")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SqlApi#provisioningListSql")
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

