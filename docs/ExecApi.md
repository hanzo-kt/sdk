# ExecApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**execExecCode**](ExecApi.md#execExecCode) | **POST** /v1/exec | Execute code in a sandboxed session |
| [**execExecProgrammatic**](ExecApi.md#execExecProgrammatic) | **POST** /v1/exec/programmatic | Programmatic code execution (sibling of /v1/exec, same executor contract) |


<a id="execExecCode"></a>
# **execExecCode**
> ExecExecResult execExecCode(execExecRequest)

Execute code in a sandboxed session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExecApi()
val execExecRequest : ExecExecRequest =  // ExecExecRequest | 
try {
    val result : ExecExecResult = apiInstance.execExecCode(execExecRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExecApi#execExecCode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExecApi#execExecCode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **execExecRequest** | [**ExecExecRequest**](ExecExecRequest.md)|  | |

### Return type

[**ExecExecResult**](ExecExecResult.md)

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

<a id="execExecProgrammatic"></a>
# **execExecProgrammatic**
> ExecExecResult execExecProgrammatic(execExecRequest)

Programmatic code execution (sibling of /v1/exec, same executor contract)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExecApi()
val execExecRequest : ExecExecRequest =  // ExecExecRequest | 
try {
    val result : ExecExecResult = apiInstance.execExecProgrammatic(execExecRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExecApi#execExecProgrammatic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExecApi#execExecProgrammatic")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **execExecRequest** | [**ExecExecRequest**](ExecExecRequest.md)|  | |

### Return type

[**ExecExecResult**](ExecExecResult.md)

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

