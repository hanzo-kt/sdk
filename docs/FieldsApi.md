# FieldsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateField**](FieldsApi.md#autoCreateField) | **POST** /v1/auto/fields | Create a field in a table |
| [**autoListFields**](FieldsApi.md#autoListFields) | **GET** /v1/auto/fields | List fields for a table |
| [**flowCreateField**](FieldsApi.md#flowCreateField) | **POST** /v1/flow/fields | Create a field in a table |
| [**flowListFields**](FieldsApi.md#flowListFields) | **GET** /v1/flow/fields | List fields for a table |


<a id="autoCreateField"></a>
# **autoCreateField**
> kotlin.Any autoCreateField(autoCreateFieldRequest)

Create a field in a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FieldsApi()
val autoCreateFieldRequest : AutoCreateFieldRequest =  // AutoCreateFieldRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateField(autoCreateFieldRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FieldsApi#autoCreateField")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FieldsApi#autoCreateField")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateFieldRequest** | [**AutoCreateFieldRequest**](AutoCreateFieldRequest.md)|  | |

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

<a id="autoListFields"></a>
# **autoListFields**
> kotlin.Any autoListFields(tableId)

List fields for a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FieldsApi()
val tableId : kotlin.String = tableId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoListFields(tableId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FieldsApi#autoListFields")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FieldsApi#autoListFields")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tableId** | **kotlin.String**|  | |

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

<a id="flowCreateField"></a>
# **flowCreateField**
> kotlin.Any flowCreateField(autoCreateFieldRequest)

Create a field in a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FieldsApi()
val autoCreateFieldRequest : AutoCreateFieldRequest =  // AutoCreateFieldRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateField(autoCreateFieldRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FieldsApi#flowCreateField")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FieldsApi#flowCreateField")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateFieldRequest** | [**AutoCreateFieldRequest**](AutoCreateFieldRequest.md)|  | |

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

<a id="flowListFields"></a>
# **flowListFields**
> kotlin.Any flowListFields(tableId)

List fields for a table

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FieldsApi()
val tableId : kotlin.String = tableId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowListFields(tableId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FieldsApi#flowListFields")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FieldsApi#flowListFields")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tableId** | **kotlin.String**|  | |

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

