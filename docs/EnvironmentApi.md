# EnvironmentApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformEnvironmentByProjectId**](EnvironmentApi.md#platformEnvironmentByProjectId) | **GET** /v1/platform/environment/byProjectId | List all environments for a project |
| [**platformEnvironmentCreate**](EnvironmentApi.md#platformEnvironmentCreate) | **POST** /v1/platform/environment/create | Create a new environment within a project |
| [**platformEnvironmentDuplicate**](EnvironmentApi.md#platformEnvironmentDuplicate) | **POST** /v1/platform/environment/duplicate | Duplicate an environment with all services |
| [**platformEnvironmentOne**](EnvironmentApi.md#platformEnvironmentOne) | **GET** /v1/platform/environment/one | Get a single environment by ID |
| [**platformEnvironmentRemove**](EnvironmentApi.md#platformEnvironmentRemove) | **POST** /v1/platform/environment/remove | Delete an environment |
| [**platformEnvironmentUpdate**](EnvironmentApi.md#platformEnvironmentUpdate) | **POST** /v1/platform/environment/update | Update an environment |


<a id="platformEnvironmentByProjectId"></a>
# **platformEnvironmentByProjectId**
> PlatformTRPCResult platformEnvironmentByProjectId(input)

List all environments for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentByProjectId(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentByProjectId")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentByProjectId")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformEnvironmentCreate"></a>
# **platformEnvironmentCreate**
> PlatformTRPCResult platformEnvironmentCreate(platformEnvironmentCreateRequest)

Create a new environment within a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val platformEnvironmentCreateRequest : PlatformEnvironmentCreateRequest =  // PlatformEnvironmentCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentCreate(platformEnvironmentCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformEnvironmentCreateRequest** | [**PlatformEnvironmentCreateRequest**](PlatformEnvironmentCreateRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformEnvironmentDuplicate"></a>
# **platformEnvironmentDuplicate**
> PlatformTRPCResult platformEnvironmentDuplicate(platformEnvironmentDuplicateRequest)

Duplicate an environment with all services

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val platformEnvironmentDuplicateRequest : PlatformEnvironmentDuplicateRequest =  // PlatformEnvironmentDuplicateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentDuplicate(platformEnvironmentDuplicateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentDuplicate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentDuplicate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformEnvironmentDuplicateRequest** | [**PlatformEnvironmentDuplicateRequest**](PlatformEnvironmentDuplicateRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformEnvironmentOne"></a>
# **platformEnvironmentOne**
> PlatformTRPCResult platformEnvironmentOne(input)

Get a single environment by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentOne")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformEnvironmentRemove"></a>
# **platformEnvironmentRemove**
> PlatformTRPCResult platformEnvironmentRemove(platformEnvironmentRemoveRequest)

Delete an environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val platformEnvironmentRemoveRequest : PlatformEnvironmentRemoveRequest =  // PlatformEnvironmentRemoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentRemove(platformEnvironmentRemoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentRemove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentRemove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformEnvironmentRemoveRequest** | [**PlatformEnvironmentRemoveRequest**](PlatformEnvironmentRemoveRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformEnvironmentUpdate"></a>
# **platformEnvironmentUpdate**
> PlatformTRPCResult platformEnvironmentUpdate(platformEnvironmentUpdateRequest)

Update an environment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EnvironmentApi()
val platformEnvironmentUpdateRequest : PlatformEnvironmentUpdateRequest =  // PlatformEnvironmentUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformEnvironmentUpdate(platformEnvironmentUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EnvironmentApi#platformEnvironmentUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EnvironmentApi#platformEnvironmentUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformEnvironmentUpdateRequest** | [**PlatformEnvironmentUpdateRequest**](PlatformEnvironmentUpdateRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

