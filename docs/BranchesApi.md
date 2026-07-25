# BranchesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dbCreateBranch**](BranchesApi.md#dbCreateBranch) | **POST** /v1/db/projects/{id}/branches | Create branch |
| [**dbDeleteBranch**](BranchesApi.md#dbDeleteBranch) | **DELETE** /v1/db/projects/{id}/branches/{branch_id} | Delete branch |
| [**dbGetBranch**](BranchesApi.md#dbGetBranch) | **GET** /v1/db/projects/{id}/branches/{branch_id} | Get branch |
| [**dbListBranches**](BranchesApi.md#dbListBranches) | **GET** /v1/db/projects/{id}/branches | List branches |
| [**dbRestoreBranch**](BranchesApi.md#dbRestoreBranch) | **POST** /v1/db/projects/{id}/branches/{branch_id}/restore | Point-in-time restore |


<a id="dbCreateBranch"></a>
# **dbCreateBranch**
> DbCreateBranch201Response dbCreateBranch(id, dbCreateBranchRequest)

Create branch

Creates an instant copy-on-write branch from the parent branch. Branching is near-instant regardless of database size. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BranchesApi()
val id : kotlin.String = id_example // kotlin.String | 
val dbCreateBranchRequest : DbCreateBranchRequest =  // DbCreateBranchRequest | 
try {
    val result : DbCreateBranch201Response = apiInstance.dbCreateBranch(id, dbCreateBranchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BranchesApi#dbCreateBranch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BranchesApi#dbCreateBranch")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbCreateBranchRequest** | [**DbCreateBranchRequest**](DbCreateBranchRequest.md)|  | |

### Return type

[**DbCreateBranch201Response**](DbCreateBranch201Response.md)

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

<a id="dbDeleteBranch"></a>
# **dbDeleteBranch**
> DbGetBranch200Response dbDeleteBranch(id, branchId)

Delete branch

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BranchesApi()
val id : kotlin.String = id_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbGetBranch200Response = apiInstance.dbDeleteBranch(id, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BranchesApi#dbDeleteBranch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BranchesApi#dbDeleteBranch")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbGetBranch200Response**](DbGetBranch200Response.md)

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

<a id="dbGetBranch"></a>
# **dbGetBranch**
> DbGetBranch200Response dbGetBranch(id, branchId)

Get branch

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BranchesApi()
val id : kotlin.String = id_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbGetBranch200Response = apiInstance.dbGetBranch(id, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BranchesApi#dbGetBranch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BranchesApi#dbGetBranch")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbGetBranch200Response**](DbGetBranch200Response.md)

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

<a id="dbListBranches"></a>
# **dbListBranches**
> DbListBranches200Response dbListBranches(id)

List branches

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BranchesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : DbListBranches200Response = apiInstance.dbListBranches(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BranchesApi#dbListBranches")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BranchesApi#dbListBranches")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**DbListBranches200Response**](DbListBranches200Response.md)

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

<a id="dbRestoreBranch"></a>
# **dbRestoreBranch**
> DbRestoreBranch200Response dbRestoreBranch(id, branchId, dbRestoreBranchRequest)

Point-in-time restore

Restore a branch to a specific point in time or LSN. Uses WAL history for precise recovery. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BranchesApi()
val id : kotlin.String = id_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
val dbRestoreBranchRequest : DbRestoreBranchRequest =  // DbRestoreBranchRequest | 
try {
    val result : DbRestoreBranch200Response = apiInstance.dbRestoreBranch(id, branchId, dbRestoreBranchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BranchesApi#dbRestoreBranch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BranchesApi#dbRestoreBranch")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **branchId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbRestoreBranchRequest** | [**DbRestoreBranchRequest**](DbRestoreBranchRequest.md)|  | |

### Return type

[**DbRestoreBranch200Response**](DbRestoreBranch200Response.md)

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

