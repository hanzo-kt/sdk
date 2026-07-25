# ProjectMembersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListProjectMembers**](ProjectMembersApi.md#autoListProjectMembers) | **GET** /v1/auto/project-members | List project members (EE) |
| [**flowAddProjectMember**](ProjectMembersApi.md#flowAddProjectMember) | **POST** /v1/flow/project-members | Add a project member (EE) |
| [**flowListProjectMembers**](ProjectMembersApi.md#flowListProjectMembers) | **GET** /v1/flow/project-members | List project members (EE) |
| [**flowRemoveProjectMember**](ProjectMembersApi.md#flowRemoveProjectMember) | **DELETE** /v1/flow/project-members/{id} | Remove a project member (EE) |


<a id="autoListProjectMembers"></a>
# **autoListProjectMembers**
> kotlin.Any autoListProjectMembers()

List project members (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectMembersApi()
try {
    val result : kotlin.Any = apiInstance.autoListProjectMembers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectMembersApi#autoListProjectMembers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectMembersApi#autoListProjectMembers")
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

<a id="flowAddProjectMember"></a>
# **flowAddProjectMember**
> kotlin.Any flowAddProjectMember(flowAddProjectMemberRequest)

Add a project member (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectMembersApi()
val flowAddProjectMemberRequest : FlowAddProjectMemberRequest =  // FlowAddProjectMemberRequest | 
try {
    val result : kotlin.Any = apiInstance.flowAddProjectMember(flowAddProjectMemberRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectMembersApi#flowAddProjectMember")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectMembersApi#flowAddProjectMember")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowAddProjectMemberRequest** | [**FlowAddProjectMemberRequest**](FlowAddProjectMemberRequest.md)|  | |

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

<a id="flowListProjectMembers"></a>
# **flowListProjectMembers**
> kotlin.Any flowListProjectMembers()

List project members (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectMembersApi()
try {
    val result : kotlin.Any = apiInstance.flowListProjectMembers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectMembersApi#flowListProjectMembers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectMembersApi#flowListProjectMembers")
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

<a id="flowRemoveProjectMember"></a>
# **flowRemoveProjectMember**
> flowRemoveProjectMember(id)

Remove a project member (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectMembersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowRemoveProjectMember(id)
} catch (e: ClientException) {
    println("4xx response calling ProjectMembersApi#flowRemoveProjectMember")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectMembersApi#flowRemoveProjectMember")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

