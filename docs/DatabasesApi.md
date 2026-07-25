# DatabasesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**dbCreateDatabase**](DatabasesApi.md#dbCreateDatabase) | **POST** /v1/db/projects/{id}/databases | Create database |
| [**dbDeleteDatabase**](DatabasesApi.md#dbDeleteDatabase) | **DELETE** /v1/db/projects/{id}/databases/{name} | Delete database |
| [**dbGetDatabase**](DatabasesApi.md#dbGetDatabase) | **GET** /v1/db/projects/{id}/databases/{name} | Get database |
| [**dbListDatabases**](DatabasesApi.md#dbListDatabases) | **GET** /v1/db/projects/{id}/databases | List databases |
| [**dbUpdateDatabase**](DatabasesApi.md#dbUpdateDatabase) | **PUT** /v1/db/projects/{id}/databases/{name} | Update database |


<a id="dbCreateDatabase"></a>
# **dbCreateDatabase**
> DbCreateDatabase201Response dbCreateDatabase(id, dbCreateDatabaseRequest)

Create database

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatabasesApi()
val id : kotlin.String = id_example // kotlin.String | 
val dbCreateDatabaseRequest : DbCreateDatabaseRequest =  // DbCreateDatabaseRequest | 
try {
    val result : DbCreateDatabase201Response = apiInstance.dbCreateDatabase(id, dbCreateDatabaseRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatabasesApi#dbCreateDatabase")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatabasesApi#dbCreateDatabase")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbCreateDatabaseRequest** | [**DbCreateDatabaseRequest**](DbCreateDatabaseRequest.md)|  | |

### Return type

[**DbCreateDatabase201Response**](DbCreateDatabase201Response.md)

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

<a id="dbDeleteDatabase"></a>
# **dbDeleteDatabase**
> DbCreateDatabase201Response dbDeleteDatabase(id, name, branchId)

Delete database

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatabasesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbCreateDatabase201Response = apiInstance.dbDeleteDatabase(id, name, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatabasesApi#dbDeleteDatabase")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatabasesApi#dbDeleteDatabase")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbCreateDatabase201Response**](DbCreateDatabase201Response.md)

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

<a id="dbGetDatabase"></a>
# **dbGetDatabase**
> DbCreateDatabase201Response dbGetDatabase(id, name, branchId)

Get database

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatabasesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbCreateDatabase201Response = apiInstance.dbGetDatabase(id, name, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatabasesApi#dbGetDatabase")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatabasesApi#dbGetDatabase")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbCreateDatabase201Response**](DbCreateDatabase201Response.md)

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

<a id="dbListDatabases"></a>
# **dbListDatabases**
> DbListDatabases200Response dbListDatabases(id, branchId)

List databases

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatabasesApi()
val id : kotlin.String = id_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbListDatabases200Response = apiInstance.dbListDatabases(id, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatabasesApi#dbListDatabases")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatabasesApi#dbListDatabases")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbListDatabases200Response**](DbListDatabases200Response.md)

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

<a id="dbUpdateDatabase"></a>
# **dbUpdateDatabase**
> DbCreateDatabase201Response dbUpdateDatabase(id, name, dbUpdateDatabaseRequest)

Update database

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatabasesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val dbUpdateDatabaseRequest : DbUpdateDatabaseRequest =  // DbUpdateDatabaseRequest | 
try {
    val result : DbCreateDatabase201Response = apiInstance.dbUpdateDatabase(id, name, dbUpdateDatabaseRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatabasesApi#dbUpdateDatabase")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatabasesApi#dbUpdateDatabase")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbUpdateDatabaseRequest** | [**DbUpdateDatabaseRequest**](DbUpdateDatabaseRequest.md)|  | |

### Return type

[**DbCreateDatabase201Response**](DbCreateDatabase201Response.md)

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

