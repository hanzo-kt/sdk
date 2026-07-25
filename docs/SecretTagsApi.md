# SecretTagsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSecretTag**](SecretTagsApi.md#kmsCreateSecretTag) | **POST** /v1/kms/projects/{projectId}/tags | Create a secret tag |
| [**kmsDeleteSecretTag**](SecretTagsApi.md#kmsDeleteSecretTag) | **DELETE** /v1/kms/projects/{projectId}/tags/{tagId} | Delete a secret tag |
| [**kmsGetSecretTag**](SecretTagsApi.md#kmsGetSecretTag) | **GET** /v1/kms/projects/{projectId}/tags/{tagId} | Get a secret tag by ID |
| [**kmsListSecretTags**](SecretTagsApi.md#kmsListSecretTags) | **GET** /v1/kms/projects/{projectId}/tags | List secret tags for a project |
| [**kmsUpdateSecretTag**](SecretTagsApi.md#kmsUpdateSecretTag) | **PATCH** /v1/kms/projects/{projectId}/tags/{tagId} | Update a secret tag |


<a id="kmsCreateSecretTag"></a>
# **kmsCreateSecretTag**
> KmsCreateSecretTag200Response kmsCreateSecretTag(projectId, kmsCreateSecretTagRequest)

Create a secret tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretTagsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsCreateSecretTagRequest : KmsCreateSecretTagRequest =  // KmsCreateSecretTagRequest | 
try {
    val result : KmsCreateSecretTag200Response = apiInstance.kmsCreateSecretTag(projectId, kmsCreateSecretTagRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretTagsApi#kmsCreateSecretTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretTagsApi#kmsCreateSecretTag")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSecretTagRequest** | [**KmsCreateSecretTagRequest**](KmsCreateSecretTagRequest.md)|  | |

### Return type

[**KmsCreateSecretTag200Response**](KmsCreateSecretTag200Response.md)

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

<a id="kmsDeleteSecretTag"></a>
# **kmsDeleteSecretTag**
> kotlin.Any kmsDeleteSecretTag(projectId, tagId)

Delete a secret tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretTagsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val tagId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteSecretTag(projectId, tagId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretTagsApi#kmsDeleteSecretTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretTagsApi#kmsDeleteSecretTag")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tagId** | **java.util.UUID**|  | |

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

<a id="kmsGetSecretTag"></a>
# **kmsGetSecretTag**
> KmsCreateSecretTag200Response kmsGetSecretTag(projectId, tagId)

Get a secret tag by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretTagsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val tagId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateSecretTag200Response = apiInstance.kmsGetSecretTag(projectId, tagId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretTagsApi#kmsGetSecretTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretTagsApi#kmsGetSecretTag")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tagId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateSecretTag200Response**](KmsCreateSecretTag200Response.md)

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

<a id="kmsListSecretTags"></a>
# **kmsListSecretTags**
> KmsListSecretTags200Response kmsListSecretTags(projectId)

List secret tags for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretTagsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListSecretTags200Response = apiInstance.kmsListSecretTags(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretTagsApi#kmsListSecretTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretTagsApi#kmsListSecretTags")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

### Return type

[**KmsListSecretTags200Response**](KmsListSecretTags200Response.md)

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

<a id="kmsUpdateSecretTag"></a>
# **kmsUpdateSecretTag**
> KmsCreateSecretTag200Response kmsUpdateSecretTag(projectId, tagId, kmsUpdateSecretTagRequest)

Update a secret tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretTagsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val tagId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateSecretTagRequest : KmsUpdateSecretTagRequest =  // KmsUpdateSecretTagRequest | 
try {
    val result : KmsCreateSecretTag200Response = apiInstance.kmsUpdateSecretTag(projectId, tagId, kmsUpdateSecretTagRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretTagsApi#kmsUpdateSecretTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretTagsApi#kmsUpdateSecretTag")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| **tagId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateSecretTagRequest** | [**KmsUpdateSecretTagRequest**](KmsUpdateSecretTagRequest.md)|  | |

### Return type

[**KmsCreateSecretTag200Response**](KmsCreateSecretTag200Response.md)

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

