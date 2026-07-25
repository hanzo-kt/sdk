# ProjectApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformProjectAll**](ProjectApi.md#platformProjectAll) | **GET** /v1/platform/project/all | List all projects in the active organization |
| [**platformProjectCreate**](ProjectApi.md#platformProjectCreate) | **POST** /v1/platform/project/create | Create a new project |
| [**platformProjectDuplicate**](ProjectApi.md#platformProjectDuplicate) | **POST** /v1/platform/project/duplicate | Duplicate a project or environment with selected services |
| [**platformProjectOne**](ProjectApi.md#platformProjectOne) | **GET** /v1/platform/project/one | Get a single project by ID |
| [**platformProjectRemove**](ProjectApi.md#platformProjectRemove) | **POST** /v1/platform/project/remove | Delete a project |
| [**platformProjectUpdate**](ProjectApi.md#platformProjectUpdate) | **POST** /v1/platform/project/update | Update a project |


<a id="platformProjectAll"></a>
# **platformProjectAll**
> PlatformTRPCResult platformProjectAll()

List all projects in the active organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="platformProjectCreate"></a>
# **platformProjectCreate**
> PlatformTRPCResult platformProjectCreate(platformProjectCreateRequest)

Create a new project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
val platformProjectCreateRequest : PlatformProjectCreateRequest =  // PlatformProjectCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectCreate(platformProjectCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformProjectCreateRequest** | [**PlatformProjectCreateRequest**](PlatformProjectCreateRequest.md)|  | |

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

<a id="platformProjectDuplicate"></a>
# **platformProjectDuplicate**
> PlatformTRPCResult platformProjectDuplicate(platformProjectDuplicateRequest)

Duplicate a project or environment with selected services

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
val platformProjectDuplicateRequest : PlatformProjectDuplicateRequest =  // PlatformProjectDuplicateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectDuplicate(platformProjectDuplicateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectDuplicate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectDuplicate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformProjectDuplicateRequest** | [**PlatformProjectDuplicateRequest**](PlatformProjectDuplicateRequest.md)|  | |

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

<a id="platformProjectOne"></a>
# **platformProjectOne**
> PlatformTRPCResult platformProjectOne(input)

Get a single project by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectOne")
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

<a id="platformProjectRemove"></a>
# **platformProjectRemove**
> PlatformTRPCResult platformProjectRemove(platformProjectRemoveRequest)

Delete a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
val platformProjectRemoveRequest : PlatformProjectRemoveRequest =  // PlatformProjectRemoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectRemove(platformProjectRemoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectRemove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectRemove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformProjectRemoveRequest** | [**PlatformProjectRemoveRequest**](PlatformProjectRemoveRequest.md)|  | |

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

<a id="platformProjectUpdate"></a>
# **platformProjectUpdate**
> PlatformTRPCResult platformProjectUpdate(platformProjectUpdateRequest)

Update a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectApi()
val platformProjectUpdateRequest : PlatformProjectUpdateRequest =  // PlatformProjectUpdateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformProjectUpdate(platformProjectUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectApi#platformProjectUpdate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectApi#platformProjectUpdate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformProjectUpdateRequest** | [**PlatformProjectUpdateRequest**](PlatformProjectUpdateRequest.md)|  | |

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

