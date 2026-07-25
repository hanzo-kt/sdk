# OrganizationApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformOrganizationAll**](OrganizationApi.md#platformOrganizationAll) | **GET** /v1/platform/organization/all | List organizations |
| [**platformOrganizationCreate**](OrganizationApi.md#platformOrganizationCreate) | **POST** /v1/platform/organization/create | Create an organization |


<a id="platformOrganizationAll"></a>
# **platformOrganizationAll**
> PlatformTRPCResult platformOrganizationAll()

List organizations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformOrganizationAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationApi#platformOrganizationAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationApi#platformOrganizationAll")
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

<a id="platformOrganizationCreate"></a>
# **platformOrganizationCreate**
> PlatformTRPCResult platformOrganizationCreate(platformOrganizationCreateRequest)

Create an organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationApi()
val platformOrganizationCreateRequest : PlatformOrganizationCreateRequest =  // PlatformOrganizationCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformOrganizationCreate(platformOrganizationCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationApi#platformOrganizationCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationApi#platformOrganizationCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformOrganizationCreateRequest** | [**PlatformOrganizationCreateRequest**](PlatformOrganizationCreateRequest.md)|  | |

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

