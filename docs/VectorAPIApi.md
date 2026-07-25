# VectorAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddVector**](VectorAPIApi.md#cloudApiControllerAddVector) | **POST** /v1/cloud/add-vector | Api Controller Add Vector |
| [**cloudApiControllerDeleteAllVectors**](VectorAPIApi.md#cloudApiControllerDeleteAllVectors) | **POST** /v1/cloud/delete-all-vectors | Api Controller Delete All Vectors |
| [**cloudApiControllerDeleteVector**](VectorAPIApi.md#cloudApiControllerDeleteVector) | **POST** /v1/cloud/delete-vector | Api Controller Delete Vector |
| [**cloudApiControllerGetGlobalVectors**](VectorAPIApi.md#cloudApiControllerGetGlobalVectors) | **GET** /v1/cloud/get-global-vectors | Api Controller Get Global Vectors |
| [**cloudApiControllerGetVectors**](VectorAPIApi.md#cloudApiControllerGetVectors) | **GET** /v1/cloud/get-vectors | Api Controller Get Vectors |
| [**cloudApiControllerUpdateVector**](VectorAPIApi.md#cloudApiControllerUpdateVector) | **POST** /v1/cloud/update-vector | Api Controller Update Vector |
| [**nexusAddVector**](VectorAPIApi.md#nexusAddVector) | **POST** /v1/nexus/add-vector | add Vector |
| [**nexusDeleteAllVectors**](VectorAPIApi.md#nexusDeleteAllVectors) | **POST** /v1/nexus/delete-all-vectors | delete All Vectors |
| [**nexusDeleteVector**](VectorAPIApi.md#nexusDeleteVector) | **POST** /v1/nexus/delete-vector | delete Vector |
| [**nexusGetGlobalVectors**](VectorAPIApi.md#nexusGetGlobalVectors) | **GET** /v1/nexus/get-global-vectors | get Global Vectors |
| [**nexusGetVectors**](VectorAPIApi.md#nexusGetVectors) | **GET** /v1/nexus/get-vectors | get Vectors |
| [**nexusUpdateVector**](VectorAPIApi.md#nexusUpdateVector) | **POST** /v1/nexus/update-vector | update Vector |


<a id="cloudApiControllerAddVector"></a>
# **cloudApiControllerAddVector**
> CloudControllersResponse cloudApiControllerAddVector(cloudObjectVector)

Api Controller Add Vector

add vector

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddVector(cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerAddVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerAddVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

<a id="cloudApiControllerDeleteAllVectors"></a>
# **cloudApiControllerDeleteAllVectors**
> CloudControllersResponse cloudApiControllerDeleteAllVectors()

Api Controller Delete All Vectors

delete all vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteAllVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerDeleteAllVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerDeleteAllVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="cloudApiControllerDeleteVector"></a>
# **cloudApiControllerDeleteVector**
> CloudControllersResponse cloudApiControllerDeleteVector(cloudObjectVector)

Api Controller Delete Vector

delete vector

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteVector(cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerDeleteVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerDeleteVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

<a id="cloudApiControllerGetGlobalVectors"></a>
# **cloudApiControllerGetGlobalVectors**
> kotlin.collections.List&lt;CloudObjectVector&gt; cloudApiControllerGetGlobalVectors()

Api Controller Get Global Vectors

get global vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectVector> = apiInstance.cloudApiControllerGetGlobalVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerGetGlobalVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerGetGlobalVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectVector&gt;**](CloudObjectVector.md)

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

<a id="cloudApiControllerGetVectors"></a>
# **cloudApiControllerGetVectors**
> kotlin.collections.List&lt;CloudObjectVector&gt; cloudApiControllerGetVectors()

Api Controller Get Vectors

get vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectVector> = apiInstance.cloudApiControllerGetVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerGetVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerGetVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectVector&gt;**](CloudObjectVector.md)

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

<a id="cloudApiControllerUpdateVector"></a>
# **cloudApiControllerUpdateVector**
> CloudControllersResponse cloudApiControllerUpdateVector(id, cloudObjectVector)

Api Controller Update Vector

update vector

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the vector
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateVector(id, cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#cloudApiControllerUpdateVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#cloudApiControllerUpdateVector")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the vector | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

<a id="nexusAddVector"></a>
# **nexusAddVector**
> NexusResponse nexusAddVector(cloudObjectVector)

add Vector

Add a vector embedding

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : NexusResponse = apiInstance.nexusAddVector(cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusAddVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusAddVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

<a id="nexusDeleteAllVectors"></a>
# **nexusDeleteAllVectors**
> NexusResponse nexusDeleteAllVectors()

delete All Vectors

Delete all vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : NexusResponse = apiInstance.nexusDeleteAllVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusDeleteAllVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusDeleteAllVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="nexusDeleteVector"></a>
# **nexusDeleteVector**
> NexusResponse nexusDeleteVector(cloudObjectVector)

delete Vector

Delete a vector embedding

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : NexusResponse = apiInstance.nexusDeleteVector(cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusDeleteVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusDeleteVector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

<a id="nexusGetGlobalVectors"></a>
# **nexusGetGlobalVectors**
> kotlin.collections.List&lt;CloudObjectVector&gt; nexusGetGlobalVectors()

get Global Vectors

Get global vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectVector> = apiInstance.nexusGetGlobalVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusGetGlobalVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusGetGlobalVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectVector&gt;**](CloudObjectVector.md)

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

<a id="nexusGetVectors"></a>
# **nexusGetVectors**
> kotlin.collections.List&lt;CloudObjectVector&gt; nexusGetVectors()

get Vectors

Get vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectVector> = apiInstance.nexusGetVectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusGetVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusGetVectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectVector&gt;**](CloudObjectVector.md)

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

<a id="nexusUpdateVector"></a>
# **nexusUpdateVector**
> NexusResponse nexusUpdateVector(id, cloudObjectVector)

update Vector

Update a vector embedding

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VectorAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the vector
val cloudObjectVector : CloudObjectVector =  // CloudObjectVector | The details of the vector
try {
    val result : NexusResponse = apiInstance.nexusUpdateVector(id, cloudObjectVector)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VectorAPIApi#nexusUpdateVector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VectorAPIApi#nexusUpdateVector")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the vector | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVector** | [**CloudObjectVector**](CloudObjectVector.md)| The details of the vector | |

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

