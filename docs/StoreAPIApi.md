# StoreAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddStore**](StoreAPIApi.md#cloudApiControllerAddStore) | **POST** /v1/cloud/add-store | Api Controller Add Store |
| [**cloudApiControllerDeleteStore**](StoreAPIApi.md#cloudApiControllerDeleteStore) | **POST** /v1/cloud/delete-store | Api Controller Delete Store |
| [**cloudApiControllerGetGlobalStores**](StoreAPIApi.md#cloudApiControllerGetGlobalStores) | **GET** /v1/cloud/get-global-stores | Api Controller Get Global Stores |
| [**cloudApiControllerGetStore**](StoreAPIApi.md#cloudApiControllerGetStore) | **GET** /v1/cloud/get-store | Api Controller Get Store |
| [**cloudApiControllerGetStores**](StoreAPIApi.md#cloudApiControllerGetStores) | **GET** /v1/cloud/get-stores | Api Controller Get Stores |
| [**cloudApiControllerRefreshStoreVectors**](StoreAPIApi.md#cloudApiControllerRefreshStoreVectors) | **POST** /v1/cloud/refresh-store-vectors | Api Controller Refresh Store Vectors |
| [**cloudApiControllerUpdateStore**](StoreAPIApi.md#cloudApiControllerUpdateStore) | **POST** /v1/cloud/update-store | Api Controller Update Store |
| [**nexusAddStore**](StoreAPIApi.md#nexusAddStore) | **POST** /v1/nexus/add-store | add Store |
| [**nexusDeleteStore**](StoreAPIApi.md#nexusDeleteStore) | **POST** /v1/nexus/delete-store | delete Store |
| [**nexusGetGlobalStores**](StoreAPIApi.md#nexusGetGlobalStores) | **GET** /v1/nexus/get-global-stores | get Global Stores |
| [**nexusGetStore**](StoreAPIApi.md#nexusGetStore) | **GET** /v1/nexus/get-store | get Store |
| [**nexusGetStores**](StoreAPIApi.md#nexusGetStores) | **GET** /v1/nexus/get-stores | get Stores |
| [**nexusRefreshStoreVectors**](StoreAPIApi.md#nexusRefreshStoreVectors) | **POST** /v1/nexus/refresh-store-vectors | refresh Store Vectors |
| [**nexusUpdateStore**](StoreAPIApi.md#nexusUpdateStore) | **POST** /v1/nexus/update-store | update Store |


<a id="cloudApiControllerAddStore"></a>
# **cloudApiControllerAddStore**
> CloudControllersResponse cloudApiControllerAddStore(cloudObjectStore)

Api Controller Add Store

add store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val cloudObjectStore : CloudObjectStore =  // CloudObjectStore | The details of the store
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddStore(cloudObjectStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerAddStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerAddStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectStore** | [**CloudObjectStore**](CloudObjectStore.md)| The details of the store | |

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

<a id="cloudApiControllerDeleteStore"></a>
# **cloudApiControllerDeleteStore**
> CloudControllersResponse cloudApiControllerDeleteStore(cloudObjectStore)

Api Controller Delete Store

delete store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val cloudObjectStore : CloudObjectStore =  // CloudObjectStore | The details of the store
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteStore(cloudObjectStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerDeleteStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerDeleteStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectStore** | [**CloudObjectStore**](CloudObjectStore.md)| The details of the store | |

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

<a id="cloudApiControllerGetGlobalStores"></a>
# **cloudApiControllerGetGlobalStores**
> kotlin.collections.List&lt;CloudObjectStore&gt; cloudApiControllerGetGlobalStores()

Api Controller Get Global Stores

get global stores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectStore> = apiInstance.cloudApiControllerGetGlobalStores()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerGetGlobalStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerGetGlobalStores")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectStore&gt;**](CloudObjectStore.md)

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

<a id="cloudApiControllerGetStore"></a>
# **cloudApiControllerGetStore**
> CloudObjectStore cloudApiControllerGetStore(id)

Api Controller Get Store

get store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the store
try {
    val result : CloudObjectStore = apiInstance.cloudApiControllerGetStore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerGetStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerGetStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the store | |

### Return type

[**CloudObjectStore**](CloudObjectStore.md)

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

<a id="cloudApiControllerGetStores"></a>
# **cloudApiControllerGetStores**
> kotlin.collections.List&lt;CloudObjectStore&gt; cloudApiControllerGetStores(owner)

Api Controller Get Stores

get stores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the store
try {
    val result : kotlin.collections.List<CloudObjectStore> = apiInstance.cloudApiControllerGetStores(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerGetStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerGetStores")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the store | |

### Return type

[**kotlin.collections.List&lt;CloudObjectStore&gt;**](CloudObjectStore.md)

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

<a id="cloudApiControllerRefreshStoreVectors"></a>
# **cloudApiControllerRefreshStoreVectors**
> CloudControllersResponse cloudApiControllerRefreshStoreVectors(cloudObjectStore)

Api Controller Refresh Store Vectors

refresh store vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val cloudObjectStore : CloudObjectStore =  // CloudObjectStore | The details of the store
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerRefreshStoreVectors(cloudObjectStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerRefreshStoreVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerRefreshStoreVectors")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectStore** | [**CloudObjectStore**](CloudObjectStore.md)| The details of the store | |

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

<a id="cloudApiControllerUpdateStore"></a>
# **cloudApiControllerUpdateStore**
> CloudControllersResponse cloudApiControllerUpdateStore(id, cloudObjectStore)

Api Controller Update Store

update store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the store
val cloudObjectStore : CloudObjectStore =  // CloudObjectStore | The details of the store
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateStore(id, cloudObjectStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#cloudApiControllerUpdateStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#cloudApiControllerUpdateStore")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the store | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectStore** | [**CloudObjectStore**](CloudObjectStore.md)| The details of the store | |

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

<a id="nexusAddStore"></a>
# **nexusAddStore**
> NexusResponse nexusAddStore(nexusStore)

add Store

Add a knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val nexusStore : NexusStore =  // NexusStore | The details of the store
try {
    val result : NexusResponse = apiInstance.nexusAddStore(nexusStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusAddStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusAddStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusStore** | [**NexusStore**](NexusStore.md)| The details of the store | |

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

<a id="nexusDeleteStore"></a>
# **nexusDeleteStore**
> NexusResponse nexusDeleteStore(nexusStore)

delete Store

Delete a knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val nexusStore : NexusStore =  // NexusStore | The details of the store
try {
    val result : NexusResponse = apiInstance.nexusDeleteStore(nexusStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusDeleteStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusDeleteStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusStore** | [**NexusStore**](NexusStore.md)| The details of the store | |

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

<a id="nexusGetGlobalStores"></a>
# **nexusGetGlobalStores**
> kotlin.collections.List&lt;NexusStore&gt; nexusGetGlobalStores()

get Global Stores

Get global knowledge stores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
try {
    val result : kotlin.collections.List<NexusStore> = apiInstance.nexusGetGlobalStores()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusGetGlobalStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusGetGlobalStores")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusStore&gt;**](NexusStore.md)

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

<a id="nexusGetStore"></a>
# **nexusGetStore**
> NexusStore nexusGetStore(id)

get Store

Get a knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the store
try {
    val result : NexusStore = apiInstance.nexusGetStore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusGetStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusGetStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the store | |

### Return type

[**NexusStore**](NexusStore.md)

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

<a id="nexusGetStores"></a>
# **nexusGetStores**
> kotlin.collections.List&lt;NexusStore&gt; nexusGetStores(owner)

get Stores

Get knowledge stores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the stores
try {
    val result : kotlin.collections.List<NexusStore> = apiInstance.nexusGetStores(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusGetStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusGetStores")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the stores | |

### Return type

[**kotlin.collections.List&lt;NexusStore&gt;**](NexusStore.md)

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

<a id="nexusRefreshStoreVectors"></a>
# **nexusRefreshStoreVectors**
> NexusResponse nexusRefreshStoreVectors(nexusStore)

refresh Store Vectors

Refresh store vectors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val nexusStore : NexusStore =  // NexusStore | The details of the store
try {
    val result : NexusResponse = apiInstance.nexusRefreshStoreVectors(nexusStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusRefreshStoreVectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusRefreshStoreVectors")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusStore** | [**NexusStore**](NexusStore.md)| The details of the store | |

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

<a id="nexusUpdateStore"></a>
# **nexusUpdateStore**
> NexusResponse nexusUpdateStore(id, nexusStore)

update Store

Update a knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the store
val nexusStore : NexusStore =  // NexusStore | The details of the store
try {
    val result : NexusResponse = apiInstance.nexusUpdateStore(id, nexusStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreAPIApi#nexusUpdateStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreAPIApi#nexusUpdateStore")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the store | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusStore** | [**NexusStore**](NexusStore.md)| The details of the store | |

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

