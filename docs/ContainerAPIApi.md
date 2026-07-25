# ContainerAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddContainer**](ContainerAPIApi.md#cloudApiControllerAddContainer) | **POST** /v1/cloud/add-container | Api Controller Add Container |
| [**cloudApiControllerDeleteContainer**](ContainerAPIApi.md#cloudApiControllerDeleteContainer) | **POST** /v1/cloud/delete-container | Api Controller Delete Container |
| [**cloudApiControllerGetContainer**](ContainerAPIApi.md#cloudApiControllerGetContainer) | **GET** /v1/cloud/get-container | Api Controller Get Container |
| [**cloudApiControllerGetContainers**](ContainerAPIApi.md#cloudApiControllerGetContainers) | **GET** /v1/cloud/get-containers | Api Controller Get Containers |
| [**cloudApiControllerUpdateContainer**](ContainerAPIApi.md#cloudApiControllerUpdateContainer) | **POST** /v1/cloud/update-container | Api Controller Update Container |
| [**nexusAddContainer**](ContainerAPIApi.md#nexusAddContainer) | **POST** /v1/nexus/add-container | add Container |
| [**nexusDeleteContainer**](ContainerAPIApi.md#nexusDeleteContainer) | **POST** /v1/nexus/delete-container | delete Container |
| [**nexusGetContainer**](ContainerAPIApi.md#nexusGetContainer) | **GET** /v1/nexus/get-container | get Container |
| [**nexusGetContainers**](ContainerAPIApi.md#nexusGetContainers) | **GET** /v1/nexus/get-containers | get Containers |
| [**nexusUpdateContainer**](ContainerAPIApi.md#nexusUpdateContainer) | **POST** /v1/nexus/update-container | update Container |


<a id="cloudApiControllerAddContainer"></a>
# **cloudApiControllerAddContainer**
> CloudControllersResponse cloudApiControllerAddContainer(cloudObjectContainer)

Api Controller Add Container

add a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddContainer(cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#cloudApiControllerAddContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#cloudApiControllerAddContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

<a id="cloudApiControllerDeleteContainer"></a>
# **cloudApiControllerDeleteContainer**
> CloudControllersResponse cloudApiControllerDeleteContainer(cloudObjectContainer)

Api Controller Delete Container

delete a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteContainer(cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#cloudApiControllerDeleteContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#cloudApiControllerDeleteContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

<a id="cloudApiControllerGetContainer"></a>
# **cloudApiControllerGetContainer**
> CloudObjectContainer cloudApiControllerGetContainer(id)

Api Controller Get Container

get container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the container
try {
    val result : CloudObjectContainer = apiInstance.cloudApiControllerGetContainer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#cloudApiControllerGetContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#cloudApiControllerGetContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the container | |

### Return type

[**CloudObjectContainer**](CloudObjectContainer.md)

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

<a id="cloudApiControllerGetContainers"></a>
# **cloudApiControllerGetContainers**
> CloudObjectContainer cloudApiControllerGetContainers(pageSize, p)

Api Controller Get Containers

get all containers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectContainer = apiInstance.cloudApiControllerGetContainers(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#cloudApiControllerGetContainers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#cloudApiControllerGetContainers")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectContainer**](CloudObjectContainer.md)

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

<a id="cloudApiControllerUpdateContainer"></a>
# **cloudApiControllerUpdateContainer**
> CloudControllersResponse cloudApiControllerUpdateContainer(id, cloudObjectContainer)

Api Controller Update Container

update container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the container
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateContainer(id, cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#cloudApiControllerUpdateContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#cloudApiControllerUpdateContainer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the container | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

<a id="nexusAddContainer"></a>
# **nexusAddContainer**
> NexusResponse nexusAddContainer(cloudObjectContainer)

add Container

Add a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : NexusResponse = apiInstance.nexusAddContainer(cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#nexusAddContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#nexusAddContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

<a id="nexusDeleteContainer"></a>
# **nexusDeleteContainer**
> NexusResponse nexusDeleteContainer(cloudObjectContainer)

delete Container

Delete a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : NexusResponse = apiInstance.nexusDeleteContainer(cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#nexusDeleteContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#nexusDeleteContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

<a id="nexusGetContainer"></a>
# **nexusGetContainer**
> CloudObjectContainer nexusGetContainer(id)

get Container

Get a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the container
try {
    val result : CloudObjectContainer = apiInstance.nexusGetContainer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#nexusGetContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#nexusGetContainer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the container | |

### Return type

[**CloudObjectContainer**](CloudObjectContainer.md)

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

<a id="nexusGetContainers"></a>
# **nexusGetContainers**
> CloudObjectContainer nexusGetContainers(pageSize, p)

get Containers

Get all containers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectContainer = apiInstance.nexusGetContainers(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#nexusGetContainers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#nexusGetContainers")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectContainer**](CloudObjectContainer.md)

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

<a id="nexusUpdateContainer"></a>
# **nexusUpdateContainer**
> NexusResponse nexusUpdateContainer(id, cloudObjectContainer)

update Container

Update a container

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContainerAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the container
val cloudObjectContainer : CloudObjectContainer =  // CloudObjectContainer | The details of the container
try {
    val result : NexusResponse = apiInstance.nexusUpdateContainer(id, cloudObjectContainer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContainerAPIApi#nexusUpdateContainer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContainerAPIApi#nexusUpdateContainer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the container | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectContainer** | [**CloudObjectContainer**](CloudObjectContainer.md)| The details of the container | |

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

