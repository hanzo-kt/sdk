# PermissionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetPermissionsByresourcetypeByresourceid**](PermissionsApi.md#chatGetPermissionsByresourcetypeByresourceid) | **GET** /v1/chat/permissions/{resourceType}/{resourceId} | Get all permissions for a resource |
| [**chatGetPermissionsByresourcetypeByresourceidEffective**](PermissionsApi.md#chatGetPermissionsByresourcetypeByresourceidEffective) | **GET** /v1/chat/permissions/{resourceType}/{resourceId}/effective | Get effective permissions for a specific resource |
| [**chatGetPermissionsByresourcetypeEffectiveAll**](PermissionsApi.md#chatGetPermissionsByresourcetypeEffectiveAll) | **GET** /v1/chat/permissions/{resourceType}/effective/all | Get effective permissions for all accessible resources |
| [**chatGetPermissionsByresourcetypeRoles**](PermissionsApi.md#chatGetPermissionsByresourcetypeRoles) | **GET** /v1/chat/permissions/{resourceType}/roles | Get available roles for a resource type |
| [**chatGetPermissionsSearchPrincipals**](PermissionsApi.md#chatGetPermissionsSearchPrincipals) | **GET** /v1/chat/permissions/search-principals | Search for users and groups to grant permissions |
| [**chatPutPermissionsByresourcetypeByresourceid**](PermissionsApi.md#chatPutPermissionsByresourcetypeByresourceid) | **PUT** /v1/chat/permissions/{resourceType}/{resourceId} | Bulk update permissions for a resource |


<a id="chatGetPermissionsByresourcetypeByresourceid"></a>
# **chatGetPermissionsByresourcetypeByresourceid**
> kotlin.Any chatGetPermissionsByresourcetypeByresourceid(resourceType, resourceId)

Get all permissions for a resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val resourceType : kotlin.String = resourceType_example // kotlin.String | 
val resourceId : kotlin.String = resourceId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPermissionsByresourcetypeByresourceid(resourceType, resourceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatGetPermissionsByresourcetypeByresourceid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatGetPermissionsByresourcetypeByresourceid")
    e.printStackTrace()
}
```

### Parameters
| **resourceType** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resourceId** | **kotlin.String**|  | |

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

<a id="chatGetPermissionsByresourcetypeByresourceidEffective"></a>
# **chatGetPermissionsByresourcetypeByresourceidEffective**
> kotlin.Any chatGetPermissionsByresourcetypeByresourceidEffective(resourceType, resourceId)

Get effective permissions for a specific resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val resourceType : kotlin.String = resourceType_example // kotlin.String | 
val resourceId : kotlin.String = resourceId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPermissionsByresourcetypeByresourceidEffective(resourceType, resourceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatGetPermissionsByresourcetypeByresourceidEffective")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatGetPermissionsByresourcetypeByresourceidEffective")
    e.printStackTrace()
}
```

### Parameters
| **resourceType** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resourceId** | **kotlin.String**|  | |

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

<a id="chatGetPermissionsByresourcetypeEffectiveAll"></a>
# **chatGetPermissionsByresourcetypeEffectiveAll**
> kotlin.Any chatGetPermissionsByresourcetypeEffectiveAll(resourceType)

Get effective permissions for all accessible resources

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val resourceType : kotlin.String = resourceType_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPermissionsByresourcetypeEffectiveAll(resourceType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatGetPermissionsByresourcetypeEffectiveAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatGetPermissionsByresourcetypeEffectiveAll")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resourceType** | **kotlin.String**|  | |

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

<a id="chatGetPermissionsByresourcetypeRoles"></a>
# **chatGetPermissionsByresourcetypeRoles**
> kotlin.Any chatGetPermissionsByresourcetypeRoles(resourceType)

Get available roles for a resource type

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val resourceType : kotlin.String = resourceType_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPermissionsByresourcetypeRoles(resourceType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatGetPermissionsByresourcetypeRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatGetPermissionsByresourcetypeRoles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resourceType** | **kotlin.String**|  | |

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

<a id="chatGetPermissionsSearchPrincipals"></a>
# **chatGetPermissionsSearchPrincipals**
> kotlin.Any chatGetPermissionsSearchPrincipals(query)

Search for users and groups to grant permissions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val query : kotlin.String = query_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetPermissionsSearchPrincipals(query)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatGetPermissionsSearchPrincipals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatGetPermissionsSearchPrincipals")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **query** | **kotlin.String**|  | [optional] |

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

<a id="chatPutPermissionsByresourcetypeByresourceid"></a>
# **chatPutPermissionsByresourcetypeByresourceid**
> kotlin.Any chatPutPermissionsByresourcetypeByresourceid(resourceType, resourceId, body)

Bulk update permissions for a resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionsApi()
val resourceType : kotlin.String = resourceType_example // kotlin.String | 
val resourceId : kotlin.String = resourceId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutPermissionsByresourcetypeByresourceid(resourceType, resourceId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionsApi#chatPutPermissionsByresourcetypeByresourceid")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionsApi#chatPutPermissionsByresourcetypeByresourceid")
    e.printStackTrace()
}
```

### Parameters
| **resourceType** | **kotlin.String**|  | |
| **resourceId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

