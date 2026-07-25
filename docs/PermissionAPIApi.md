# PermissionAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddPermission**](PermissionAPIApi.md#cloudApiControllerAddPermission) | **POST** /v1/cloud/add-permission | Api Controller Add Permission |
| [**cloudApiControllerDeletePermission**](PermissionAPIApi.md#cloudApiControllerDeletePermission) | **POST** /v1/cloud/delete-permission | Api Controller Delete Permission |
| [**cloudApiControllerGetPermission**](PermissionAPIApi.md#cloudApiControllerGetPermission) | **GET** /v1/cloud/get-permission | Api Controller Get Permission |
| [**cloudApiControllerGetPermissions**](PermissionAPIApi.md#cloudApiControllerGetPermissions) | **GET** /v1/cloud/get-permissions | Api Controller Get Permissions |
| [**cloudApiControllerUpdatePermission**](PermissionAPIApi.md#cloudApiControllerUpdatePermission) | **POST** /v1/cloud/update-permission | Api Controller Update Permission |
| [**nexusAddPermission**](PermissionAPIApi.md#nexusAddPermission) | **POST** /v1/nexus/add-permission | add Permission |
| [**nexusDeletePermission**](PermissionAPIApi.md#nexusDeletePermission) | **POST** /v1/nexus/delete-permission | delete Permission |
| [**nexusGetPermission**](PermissionAPIApi.md#nexusGetPermission) | **GET** /v1/nexus/get-permission | get Permission |
| [**nexusGetPermissions**](PermissionAPIApi.md#nexusGetPermissions) | **GET** /v1/nexus/get-permissions | get Permissions |
| [**nexusUpdatePermission**](PermissionAPIApi.md#nexusUpdatePermission) | **POST** /v1/nexus/update-permission | update Permission |


<a id="cloudApiControllerAddPermission"></a>
# **cloudApiControllerAddPermission**
> CloudControllersResponse cloudApiControllerAddPermission(body)

Api Controller Add Permission

add permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddPermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#cloudApiControllerAddPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#cloudApiControllerAddPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeletePermission"></a>
# **cloudApiControllerDeletePermission**
> CloudControllersResponse cloudApiControllerDeletePermission(body)

Api Controller Delete Permission

delete permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeletePermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#cloudApiControllerDeletePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#cloudApiControllerDeletePermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetPermission"></a>
# **cloudApiControllerGetPermission**
> kotlin.Any cloudApiControllerGetPermission(id)

Api Controller Get Permission

get permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id(owner/name) of permission
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetPermission(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#cloudApiControllerGetPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#cloudApiControllerGetPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id(owner/name) of permission | |

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

<a id="cloudApiControllerGetPermissions"></a>
# **cloudApiControllerGetPermissions**
> kotlin.collections.List&lt;kotlin.Any&gt; cloudApiControllerGetPermissions()

Api Controller Get Permissions

get permissions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.cloudApiControllerGetPermissions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#cloudApiControllerGetPermissions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#cloudApiControllerGetPermissions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="cloudApiControllerUpdatePermission"></a>
# **cloudApiControllerUpdatePermission**
> CloudControllersResponse cloudApiControllerUpdatePermission(body)

Api Controller Update Permission

update permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdatePermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#cloudApiControllerUpdatePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#cloudApiControllerUpdatePermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddPermission"></a>
# **nexusAddPermission**
> NexusResponse nexusAddPermission(body)

add Permission

Add a permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : NexusResponse = apiInstance.nexusAddPermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#nexusAddPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#nexusAddPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeletePermission"></a>
# **nexusDeletePermission**
> NexusResponse nexusDeletePermission(body)

delete Permission

Delete a permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : NexusResponse = apiInstance.nexusDeletePermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#nexusDeletePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#nexusDeletePermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetPermission"></a>
# **nexusGetPermission**
> kotlin.Any nexusGetPermission(id)

get Permission

Get a permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the permission
try {
    val result : kotlin.Any = apiInstance.nexusGetPermission(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#nexusGetPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#nexusGetPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the permission | |

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

<a id="nexusGetPermissions"></a>
# **nexusGetPermissions**
> kotlin.collections.List&lt;kotlin.Any&gt; nexusGetPermissions()

get Permissions

Get permissions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.nexusGetPermissions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#nexusGetPermissions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#nexusGetPermissions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="nexusUpdatePermission"></a>
# **nexusUpdatePermission**
> NexusResponse nexusUpdatePermission(body)

update Permission

Update a permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PermissionAPIApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the permission
try {
    val result : NexusResponse = apiInstance.nexusUpdatePermission(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PermissionAPIApi#nexusUpdatePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PermissionAPIApi#nexusUpdatePermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the permission | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

