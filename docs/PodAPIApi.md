# PodAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddPod**](PodAPIApi.md#cloudApiControllerAddPod) | **POST** /v1/cloud/add-pod | Api Controller Add Pod |
| [**cloudApiControllerDeletePod**](PodAPIApi.md#cloudApiControllerDeletePod) | **POST** /v1/cloud/delete-pod | Api Controller Delete Pod |
| [**cloudApiControllerGetPod**](PodAPIApi.md#cloudApiControllerGetPod) | **GET** /v1/cloud/get-pod | Api Controller Get Pod |
| [**cloudApiControllerGetPods**](PodAPIApi.md#cloudApiControllerGetPods) | **GET** /v1/cloud/get-pods | Api Controller Get Pods |
| [**cloudApiControllerUpdatePod**](PodAPIApi.md#cloudApiControllerUpdatePod) | **POST** /v1/cloud/update-pod | Api Controller Update Pod |
| [**nexusAddPod**](PodAPIApi.md#nexusAddPod) | **POST** /v1/nexus/add-pod | add Pod |
| [**nexusDeletePod**](PodAPIApi.md#nexusDeletePod) | **POST** /v1/nexus/delete-pod | delete Pod |
| [**nexusGetPod**](PodAPIApi.md#nexusGetPod) | **GET** /v1/nexus/get-pod | get Pod |
| [**nexusGetPods**](PodAPIApi.md#nexusGetPods) | **GET** /v1/nexus/get-pods | get Pods |
| [**nexusUpdatePod**](PodAPIApi.md#nexusUpdatePod) | **POST** /v1/nexus/update-pod | update Pod |


<a id="cloudApiControllerAddPod"></a>
# **cloudApiControllerAddPod**
> CloudControllersResponse cloudApiControllerAddPod(cloudObjectPod)

Api Controller Add Pod

add a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddPod(cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#cloudApiControllerAddPod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#cloudApiControllerAddPod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

<a id="cloudApiControllerDeletePod"></a>
# **cloudApiControllerDeletePod**
> CloudControllersResponse cloudApiControllerDeletePod(cloudObjectPod)

Api Controller Delete Pod

delete a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeletePod(cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#cloudApiControllerDeletePod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#cloudApiControllerDeletePod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

<a id="cloudApiControllerGetPod"></a>
# **cloudApiControllerGetPod**
> CloudObjectPod cloudApiControllerGetPod(id)

Api Controller Get Pod

get pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the pod
try {
    val result : CloudObjectPod = apiInstance.cloudApiControllerGetPod(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#cloudApiControllerGetPod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#cloudApiControllerGetPod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the pod | |

### Return type

[**CloudObjectPod**](CloudObjectPod.md)

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

<a id="cloudApiControllerGetPods"></a>
# **cloudApiControllerGetPods**
> CloudObjectPod cloudApiControllerGetPods(pageSize, p)

Api Controller Get Pods

get all pods

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectPod = apiInstance.cloudApiControllerGetPods(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#cloudApiControllerGetPods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#cloudApiControllerGetPods")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectPod**](CloudObjectPod.md)

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

<a id="cloudApiControllerUpdatePod"></a>
# **cloudApiControllerUpdatePod**
> CloudControllersResponse cloudApiControllerUpdatePod(id, cloudObjectPod)

Api Controller Update Pod

update pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the pod
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdatePod(id, cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#cloudApiControllerUpdatePod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#cloudApiControllerUpdatePod")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the pod | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

<a id="nexusAddPod"></a>
# **nexusAddPod**
> NexusResponse nexusAddPod(cloudObjectPod)

add Pod

Add a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : NexusResponse = apiInstance.nexusAddPod(cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#nexusAddPod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#nexusAddPod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

<a id="nexusDeletePod"></a>
# **nexusDeletePod**
> NexusResponse nexusDeletePod(cloudObjectPod)

delete Pod

Delete a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : NexusResponse = apiInstance.nexusDeletePod(cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#nexusDeletePod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#nexusDeletePod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

<a id="nexusGetPod"></a>
# **nexusGetPod**
> CloudObjectPod nexusGetPod(id)

get Pod

Get a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the pod
try {
    val result : CloudObjectPod = apiInstance.nexusGetPod(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#nexusGetPod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#nexusGetPod")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the pod | |

### Return type

[**CloudObjectPod**](CloudObjectPod.md)

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

<a id="nexusGetPods"></a>
# **nexusGetPods**
> CloudObjectPod nexusGetPods(pageSize, p)

get Pods

Get all pods

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectPod = apiInstance.nexusGetPods(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#nexusGetPods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#nexusGetPods")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectPod**](CloudObjectPod.md)

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

<a id="nexusUpdatePod"></a>
# **nexusUpdatePod**
> NexusResponse nexusUpdatePod(id, cloudObjectPod)

update Pod

Update a pod

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PodAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the pod
val cloudObjectPod : CloudObjectPod =  // CloudObjectPod | The details of the pod
try {
    val result : NexusResponse = apiInstance.nexusUpdatePod(id, cloudObjectPod)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PodAPIApi#nexusUpdatePod")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PodAPIApi#nexusUpdatePod")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the pod | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectPod** | [**CloudObjectPod**](CloudObjectPod.md)| The details of the pod | |

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

