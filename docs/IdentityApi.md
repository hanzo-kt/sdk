# IdentityApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminListApplications**](IdentityApi.md#adminAdminListApplications) | **GET** /v1/admin/applications | IAM applications (verbatim passthrough) |
| [**adminAdminListOrgs**](IdentityApi.md#adminAdminListOrgs) | **GET** /v1/admin/orgs | Tenant directory |
| [**adminAdminListRoles**](IdentityApi.md#adminAdminListRoles) | **GET** /v1/admin/roles | IAM roles (verbatim passthrough) |
| [**adminAdminListUsers**](IdentityApi.md#adminAdminListUsers) | **GET** /v1/admin/users | Cross-org user directory |
| [**adminAdminMe**](IdentityApi.md#adminAdminMe) | **GET** /v1/admin/me | Validated operator identity |


<a id="adminAdminListApplications"></a>
# **adminAdminListApplications**
> AdminRawList adminAdminListApplications(owner, p, pageSize)

IAM applications (verbatim passthrough)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityApi()
val owner : kotlin.String = owner_example // kotlin.String | 
val p : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AdminRawList = apiInstance.adminAdminListApplications(owner, p, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityApi#adminAdminListApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityApi#adminAdminListApplications")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**|  | [optional] |
| **p** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**AdminRawList**](AdminRawList.md)

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

<a id="adminAdminListOrgs"></a>
# **adminAdminListOrgs**
> AdminOrgList adminAdminListOrgs()

Tenant directory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityApi()
try {
    val result : AdminOrgList = apiInstance.adminAdminListOrgs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityApi#adminAdminListOrgs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityApi#adminAdminListOrgs")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminOrgList**](AdminOrgList.md)

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

<a id="adminAdminListRoles"></a>
# **adminAdminListRoles**
> AdminRawList adminAdminListRoles(owner, p, pageSize)

IAM roles (verbatim passthrough)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityApi()
val owner : kotlin.String = owner_example // kotlin.String | 
val p : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AdminRawList = apiInstance.adminAdminListRoles(owner, p, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityApi#adminAdminListRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityApi#adminAdminListRoles")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**|  | [optional] |
| **p** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**AdminRawList**](AdminRawList.md)

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

<a id="adminAdminListUsers"></a>
# **adminAdminListUsers**
> AdminUserList adminAdminListUsers(org, p, pageSize, q)

Cross-org user directory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityApi()
val org : kotlin.String = org_example // kotlin.String | Filter to one org (owner)
val p : kotlin.Int = 56 // kotlin.Int | 1-based page
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val q : kotlin.String = q_example // kotlin.String | Free-text name filter
try {
    val result : AdminUserList = apiInstance.adminAdminListUsers(org, p, pageSize, q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityApi#adminAdminListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityApi#adminAdminListUsers")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**| Filter to one org (owner) | [optional] |
| **p** | **kotlin.Int**| 1-based page | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**| Free-text name filter | [optional] |

### Return type

[**AdminUserList**](AdminUserList.md)

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

<a id="adminAdminMe"></a>
# **adminAdminMe**
> AdminAdminMe200Response adminAdminMe()

Validated operator identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityApi()
try {
    val result : AdminAdminMe200Response = apiInstance.adminAdminMe()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityApi#adminAdminMe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityApi#adminAdminMe")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminMe200Response**](AdminAdminMe200Response.md)

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

