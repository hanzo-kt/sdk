# BindingsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**visorBindMachineAgent**](BindingsApi.md#visorBindMachineAgent) | **POST** /v1/machines/{id}/bind-agent | Bind a cloud Agent to a machine |
| [**visorGetMachineAgentBinding**](BindingsApi.md#visorGetMachineAgentBinding) | **GET** /v1/machines/{id}/agent-binding | Get a machine&#39;s agent binding |
| [**visorListAgentBindings**](BindingsApi.md#visorListAgentBindings) | **GET** /v1/agent-bindings | List the org&#39;s agent bindings |
| [**visorUnbindMachineAgent**](BindingsApi.md#visorUnbindMachineAgent) | **DELETE** /v1/machines/{id}/agent-binding | Unbind the agent from a machine |


<a id="visorBindMachineAgent"></a>
# **visorBindMachineAgent**
> VisorAgentBinding visorBindMachineAgent(id, visorBindAgentRequest)

Bind a cloud Agent to a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BindingsApi()
val id : kotlin.String = id_example // kotlin.String | 
val visorBindAgentRequest : VisorBindAgentRequest =  // VisorBindAgentRequest | 
try {
    val result : VisorAgentBinding = apiInstance.visorBindMachineAgent(id, visorBindAgentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BindingsApi#visorBindMachineAgent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BindingsApi#visorBindMachineAgent")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visorBindAgentRequest** | [**VisorBindAgentRequest**](VisorBindAgentRequest.md)|  | |

### Return type

[**VisorAgentBinding**](VisorAgentBinding.md)

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

<a id="visorGetMachineAgentBinding"></a>
# **visorGetMachineAgentBinding**
> VisorAgentBinding visorGetMachineAgentBinding(id)

Get a machine&#39;s agent binding

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BindingsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : VisorAgentBinding = apiInstance.visorGetMachineAgentBinding(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BindingsApi#visorGetMachineAgentBinding")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BindingsApi#visorGetMachineAgentBinding")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**VisorAgentBinding**](VisorAgentBinding.md)

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

<a id="visorListAgentBindings"></a>
# **visorListAgentBindings**
> VisorListAgentBindings200Response visorListAgentBindings()

List the org&#39;s agent bindings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BindingsApi()
try {
    val result : VisorListAgentBindings200Response = apiInstance.visorListAgentBindings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BindingsApi#visorListAgentBindings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BindingsApi#visorListAgentBindings")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListAgentBindings200Response**](VisorListAgentBindings200Response.md)

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

<a id="visorUnbindMachineAgent"></a>
# **visorUnbindMachineAgent**
> visorUnbindMachineAgent(id)

Unbind the agent from a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BindingsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.visorUnbindMachineAgent(id)
} catch (e: ClientException) {
    println("4xx response calling BindingsApi#visorUnbindMachineAgent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BindingsApi#visorUnbindMachineAgent")
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
 - **Accept**: application/json

