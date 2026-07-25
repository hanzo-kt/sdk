# MachineAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddMachine**](MachineAPIApi.md#cloudApiControllerAddMachine) | **POST** /v1/cloud/add-machine | Api Controller Add Machine |
| [**cloudApiControllerDeleteMachine**](MachineAPIApi.md#cloudApiControllerDeleteMachine) | **POST** /v1/cloud/delete-machine | Api Controller Delete Machine |
| [**cloudApiControllerGetMachine**](MachineAPIApi.md#cloudApiControllerGetMachine) | **GET** /v1/cloud/get-machine | Api Controller Get Machine |
| [**cloudApiControllerGetMachines**](MachineAPIApi.md#cloudApiControllerGetMachines) | **GET** /v1/cloud/get-machines | Api Controller Get Machines |
| [**cloudApiControllerUpdateMachine**](MachineAPIApi.md#cloudApiControllerUpdateMachine) | **POST** /v1/cloud/update-machine | Api Controller Update Machine |
| [**nexusAddMachine**](MachineAPIApi.md#nexusAddMachine) | **POST** /v1/nexus/add-machine | add Machine |
| [**nexusDeleteMachine**](MachineAPIApi.md#nexusDeleteMachine) | **POST** /v1/nexus/delete-machine | delete Machine |
| [**nexusGetMachine**](MachineAPIApi.md#nexusGetMachine) | **GET** /v1/nexus/get-machine | get Machine |
| [**nexusGetMachines**](MachineAPIApi.md#nexusGetMachines) | **GET** /v1/nexus/get-machines | get Machines |
| [**nexusUpdateMachine**](MachineAPIApi.md#nexusUpdateMachine) | **POST** /v1/nexus/update-machine | update Machine |


<a id="cloudApiControllerAddMachine"></a>
# **cloudApiControllerAddMachine**
> CloudControllersResponse cloudApiControllerAddMachine(cloudObjectMachine)

Api Controller Add Machine

add a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddMachine(cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#cloudApiControllerAddMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#cloudApiControllerAddMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteMachine"></a>
# **cloudApiControllerDeleteMachine**
> CloudControllersResponse cloudApiControllerDeleteMachine(cloudObjectMachine)

Api Controller Delete Machine

delete a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteMachine(cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#cloudApiControllerDeleteMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#cloudApiControllerDeleteMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetMachine"></a>
# **cloudApiControllerGetMachine**
> CloudObjectMachine cloudApiControllerGetMachine(id)

Api Controller Get Machine

get machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the machine
try {
    val result : CloudObjectMachine = apiInstance.cloudApiControllerGetMachine(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#cloudApiControllerGetMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#cloudApiControllerGetMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the machine | |

### Return type

[**CloudObjectMachine**](CloudObjectMachine.md)

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

<a id="cloudApiControllerGetMachines"></a>
# **cloudApiControllerGetMachines**
> CloudObjectMachine cloudApiControllerGetMachines(pageSize, p)

Api Controller Get Machines

get all machines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectMachine = apiInstance.cloudApiControllerGetMachines(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#cloudApiControllerGetMachines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#cloudApiControllerGetMachines")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectMachine**](CloudObjectMachine.md)

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

<a id="cloudApiControllerUpdateMachine"></a>
# **cloudApiControllerUpdateMachine**
> CloudControllersResponse cloudApiControllerUpdateMachine(id, cloudObjectMachine)

Api Controller Update Machine

update machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the machine
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateMachine(id, cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#cloudApiControllerUpdateMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#cloudApiControllerUpdateMachine")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the machine | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddMachine"></a>
# **nexusAddMachine**
> NexusResponse nexusAddMachine(cloudObjectMachine)

add Machine

Add a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : NexusResponse = apiInstance.nexusAddMachine(cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#nexusAddMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#nexusAddMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteMachine"></a>
# **nexusDeleteMachine**
> NexusResponse nexusDeleteMachine(cloudObjectMachine)

delete Machine

Delete a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : NexusResponse = apiInstance.nexusDeleteMachine(cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#nexusDeleteMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#nexusDeleteMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetMachine"></a>
# **nexusGetMachine**
> CloudObjectMachine nexusGetMachine(id)

get Machine

Get a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the machine
try {
    val result : CloudObjectMachine = apiInstance.nexusGetMachine(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#nexusGetMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#nexusGetMachine")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the machine | |

### Return type

[**CloudObjectMachine**](CloudObjectMachine.md)

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

<a id="nexusGetMachines"></a>
# **nexusGetMachines**
> CloudObjectMachine nexusGetMachines(pageSize, p)

get Machines

Get all machines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectMachine = apiInstance.nexusGetMachines(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#nexusGetMachines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#nexusGetMachines")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectMachine**](CloudObjectMachine.md)

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

<a id="nexusUpdateMachine"></a>
# **nexusUpdateMachine**
> NexusResponse nexusUpdateMachine(id, cloudObjectMachine)

update Machine

Update a machine

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MachineAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the machine
val cloudObjectMachine : CloudObjectMachine =  // CloudObjectMachine | The details of the machine
try {
    val result : NexusResponse = apiInstance.nexusUpdateMachine(id, cloudObjectMachine)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MachineAPIApi#nexusUpdateMachine")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MachineAPIApi#nexusUpdateMachine")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the machine | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectMachine** | [**CloudObjectMachine**](CloudObjectMachine.md)| The details of the machine | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

