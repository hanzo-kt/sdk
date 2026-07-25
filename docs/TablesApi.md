# TablesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateTable**](TablesApi.md#autoCreateTable) | **POST** /v1/auto/tables | Create a table |
| [**autoListTables**](TablesApi.md#autoListTables) | **GET** /v1/auto/tables | List tables |
| [**flowCreateTable**](TablesApi.md#flowCreateTable) | **POST** /v1/flow/tables | Create a table |
| [**flowDeleteTable**](TablesApi.md#flowDeleteTable) | **DELETE** /v1/flow/tables/{id} | Delete a table |
| [**flowGetTable**](TablesApi.md#flowGetTable) | **GET** /v1/flow/tables/{id} | Get a table |
| [**flowListTables**](TablesApi.md#flowListTables) | **GET** /v1/flow/tables | List tables |


<a id="autoCreateTable"></a>
# **autoCreateTable**
> kotlin.Any autoCreateTable(autoCreateTableRequest)

Create a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
val autoCreateTableRequest : AutoCreateTableRequest =  // AutoCreateTableRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateTable(autoCreateTableRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#autoCreateTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#autoCreateTable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateTableRequest** | [**AutoCreateTableRequest**](AutoCreateTableRequest.md)|  | |

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

<a id="autoListTables"></a>
# **autoListTables**
> kotlin.Any autoListTables()

List tables

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
try {
    val result : kotlin.Any = apiInstance.autoListTables()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#autoListTables")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#autoListTables")
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

<a id="flowCreateTable"></a>
# **flowCreateTable**
> kotlin.Any flowCreateTable(autoCreateTableRequest)

Create a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
val autoCreateTableRequest : AutoCreateTableRequest =  // AutoCreateTableRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateTable(autoCreateTableRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#flowCreateTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#flowCreateTable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateTableRequest** | [**AutoCreateTableRequest**](AutoCreateTableRequest.md)|  | |

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

<a id="flowDeleteTable"></a>
# **flowDeleteTable**
> flowDeleteTable(id)

Delete a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteTable(id)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#flowDeleteTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#flowDeleteTable")
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

<a id="flowGetTable"></a>
# **flowGetTable**
> kotlin.Any flowGetTable(id)

Get a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetTable(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#flowGetTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#flowGetTable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowListTables"></a>
# **flowListTables**
> kotlin.Any flowListTables()

List tables

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TablesApi()
try {
    val result : kotlin.Any = apiInstance.flowListTables()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TablesApi#flowListTables")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TablesApi#flowListTables")
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

