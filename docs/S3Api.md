# S3Api

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**provisioningCreateS3**](S3Api.md#provisioningCreateS3) | **POST** /v1/s3 | Provision an object-storage bucket |
| [**provisioningDeleteS3**](S3Api.md#provisioningDeleteS3) | **DELETE** /v1/s3/{name} | Deprovision an object-storage bucket |
| [**provisioningGetS3**](S3Api.md#provisioningGetS3) | **GET** /v1/s3/{name} | Get one object-storage bucket |
| [**provisioningListS3**](S3Api.md#provisioningListS3) | **GET** /v1/s3 | List object-storage buckets for the caller&#39;s org |


<a id="provisioningCreateS3"></a>
# **provisioningCreateS3**
> ProvisioningCreateResponse provisioningCreateS3(provisioningCreateRequest)

Provision an object-storage bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = S3Api()
val provisioningCreateRequest : ProvisioningCreateRequest =  // ProvisioningCreateRequest | 
try {
    val result : ProvisioningCreateResponse = apiInstance.provisioningCreateS3(provisioningCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling S3Api#provisioningCreateS3")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling S3Api#provisioningCreateS3")
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

<a id="provisioningDeleteS3"></a>
# **provisioningDeleteS3**
> provisioningDeleteS3(name)

Deprovision an object-storage bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = S3Api()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    apiInstance.provisioningDeleteS3(name)
} catch (e: ClientException) {
    println("4xx response calling S3Api#provisioningDeleteS3")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling S3Api#provisioningDeleteS3")
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

<a id="provisioningGetS3"></a>
# **provisioningGetS3**
> ProvisioningGetResponse provisioningGetS3(name)

Get one object-storage bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = S3Api()
val name : kotlin.String = name_example // kotlin.String | The user-supplied resource name (slug). Lowercased and trimmed server-side; must match `^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$`. 
try {
    val result : ProvisioningGetResponse = apiInstance.provisioningGetS3(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling S3Api#provisioningGetS3")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling S3Api#provisioningGetS3")
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

<a id="provisioningListS3"></a>
# **provisioningListS3**
> kotlin.collections.List&lt;ProvisioningListItem&gt; provisioningListS3()

List object-storage buckets for the caller&#39;s org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = S3Api()
try {
    val result : kotlin.collections.List<ProvisioningListItem> = apiInstance.provisioningListS3()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling S3Api#provisioningListS3")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling S3Api#provisioningListS3")
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

