# TodosApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListTodos**](TodosApi.md#autoListTodos) | **GET** /v1/auto/todos | List todos |
| [**flowGetTodo**](TodosApi.md#flowGetTodo) | **GET** /v1/flow/todos/{id} | Get a todo |
| [**flowListTodoActivities**](TodosApi.md#flowListTodoActivities) | **GET** /v1/flow/todo-activities | List todo activity log |
| [**flowListTodos**](TodosApi.md#flowListTodos) | **GET** /v1/flow/todos | List todos |
| [**flowUpdateTodo**](TodosApi.md#flowUpdateTodo) | **POST** /v1/flow/todos/{id} | Update a todo |


<a id="autoListTodos"></a>
# **autoListTodos**
> kotlin.Any autoListTodos()

List todos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TodosApi()
try {
    val result : kotlin.Any = apiInstance.autoListTodos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TodosApi#autoListTodos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TodosApi#autoListTodos")
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

<a id="flowGetTodo"></a>
# **flowGetTodo**
> kotlin.Any flowGetTodo(id)

Get a todo

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TodosApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetTodo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TodosApi#flowGetTodo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TodosApi#flowGetTodo")
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

<a id="flowListTodoActivities"></a>
# **flowListTodoActivities**
> kotlin.Any flowListTodoActivities(todoId)

List todo activity log

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TodosApi()
val todoId : kotlin.String = todoId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowListTodoActivities(todoId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TodosApi#flowListTodoActivities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TodosApi#flowListTodoActivities")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **todoId** | **kotlin.String**|  | |

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

<a id="flowListTodos"></a>
# **flowListTodos**
> kotlin.Any flowListTodos(cursor, limit)

List todos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TodosApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.flowListTodos(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TodosApi#flowListTodos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TodosApi#flowListTodos")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

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

<a id="flowUpdateTodo"></a>
# **flowUpdateTodo**
> kotlin.Any flowUpdateTodo(id, flowUpdateTodoRequest)

Update a todo

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TodosApi()
val id : kotlin.String = id_example // kotlin.String | 
val flowUpdateTodoRequest : FlowUpdateTodoRequest =  // FlowUpdateTodoRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpdateTodo(id, flowUpdateTodoRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TodosApi#flowUpdateTodo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TodosApi#flowUpdateTodo")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpdateTodoRequest** | [**FlowUpdateTodoRequest**](FlowUpdateTodoRequest.md)|  | |

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

