# ProjectRolesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListProjectRoles**](ProjectRolesApi.md#autoListProjectRoles) | **GET** /v1/auto/project-roles | List project roles (EE) |
| [**flowListProjectRoles**](ProjectRolesApi.md#flowListProjectRoles) | **GET** /v1/flow/project-roles | List project roles (EE) |


<a id="autoListProjectRoles"></a>
# **autoListProjectRoles**
> kotlin.Any autoListProjectRoles()

List project roles (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectRolesApi()
try {
    val result : kotlin.Any = apiInstance.autoListProjectRoles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectRolesApi#autoListProjectRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectRolesApi#autoListProjectRoles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="flowListProjectRoles"></a>
# **flowListProjectRoles**
> kotlin.Any flowListProjectRoles()

List project roles (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectRolesApi()
try {
    val result : kotlin.Any = apiInstance.flowListProjectRoles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectRolesApi#flowListProjectRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectRolesApi#flowListProjectRoles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

