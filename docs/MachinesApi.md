# MachinesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**visorDeleteMachine**](MachinesApi.md#visorDeleteMachine) | **DELETE** /v1/machines/{id} | Terminate a machine |
| [**visorGetMachine**](MachinesApi.md#visorGetMachine) | **GET** /v1/machines/{id} | Get one machine by org-scoped name |
| [**visorLaunchMachine**](MachinesApi.md#visorLaunchMachine) | **POST** /v1/machines | Launch a machine (or dryRun for a price quote) |
| [**visorListMachines**](MachinesApi.md#visorListMachines) | **GET** /v1/machines | List the org&#39;s machines |


<a id="visorDeleteMachine"></a>
# **visorDeleteMachine**
> visorDeleteMachine(id)

Terminate a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachinesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.visorDeleteMachine(id)
} catch (e: ClientException) {
    println("4xx response calling MachinesApi#visorDeleteMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachinesApi#visorDeleteMachine")
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

<a id="visorGetMachine"></a>
# **visorGetMachine**
> VisorMachineView visorGetMachine(id)

Get one machine by org-scoped name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachinesApi()
val id : kotlin.String = id_example // kotlin.String | Org-scoped machine name
try {
    val result : VisorMachineView = apiInstance.visorGetMachine(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachinesApi#visorGetMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachinesApi#visorGetMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Org-scoped machine name | |

### Return type

[**VisorMachineView**](VisorMachineView.md)

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

<a id="visorLaunchMachine"></a>
# **visorLaunchMachine**
> kotlin.Any visorLaunchMachine(visorLaunchRequest)

Launch a machine (or dryRun for a price quote)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachinesApi()
val visorLaunchRequest : VisorLaunchRequest =  // VisorLaunchRequest | 
try {
    val result : kotlin.Any = apiInstance.visorLaunchMachine(visorLaunchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachinesApi#visorLaunchMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachinesApi#visorLaunchMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **visorLaunchRequest** | [**VisorLaunchRequest**](VisorLaunchRequest.md)|  | |

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

<a id="visorListMachines"></a>
# **visorListMachines**
> VisorListMachines200Response visorListMachines()

List the org&#39;s machines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachinesApi()
try {
    val result : VisorListMachines200Response = apiInstance.visorListMachines()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachinesApi#visorListMachines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachinesApi#visorListMachines")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListMachines200Response**](VisorListMachines200Response.md)

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

