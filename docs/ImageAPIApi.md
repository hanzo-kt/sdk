# ImageAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddImage**](ImageAPIApi.md#cloudApiControllerAddImage) | **POST** /v1/cloud/add-image | Api Controller Add Image |
| [**cloudApiControllerDeleteImage**](ImageAPIApi.md#cloudApiControllerDeleteImage) | **POST** /v1/cloud/delete-image | Api Controller Delete Image |
| [**cloudApiControllerGetImage**](ImageAPIApi.md#cloudApiControllerGetImage) | **GET** /v1/cloud/get-image | Api Controller Get Image |
| [**cloudApiControllerGetImages**](ImageAPIApi.md#cloudApiControllerGetImages) | **GET** /v1/cloud/get-images | Api Controller Get Images |
| [**cloudApiControllerUpdateImage**](ImageAPIApi.md#cloudApiControllerUpdateImage) | **POST** /v1/cloud/update-image | Api Controller Update Image |
| [**nexusAddImage**](ImageAPIApi.md#nexusAddImage) | **POST** /v1/nexus/add-image | add Image |
| [**nexusDeleteImage**](ImageAPIApi.md#nexusDeleteImage) | **POST** /v1/nexus/delete-image | delete Image |
| [**nexusGetImage**](ImageAPIApi.md#nexusGetImage) | **GET** /v1/nexus/get-image | get Image |
| [**nexusGetImages**](ImageAPIApi.md#nexusGetImages) | **GET** /v1/nexus/get-images | get Images |
| [**nexusUpdateImage**](ImageAPIApi.md#nexusUpdateImage) | **POST** /v1/nexus/update-image | update Image |


<a id="cloudApiControllerAddImage"></a>
# **cloudApiControllerAddImage**
> CloudControllersResponse cloudApiControllerAddImage(cloudObjectImage)

Api Controller Add Image

add a image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddImage(cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#cloudApiControllerAddImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#cloudApiControllerAddImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

<a id="cloudApiControllerDeleteImage"></a>
# **cloudApiControllerDeleteImage**
> CloudControllersResponse cloudApiControllerDeleteImage(cloudObjectImage)

Api Controller Delete Image

delete a image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteImage(cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#cloudApiControllerDeleteImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#cloudApiControllerDeleteImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

<a id="cloudApiControllerGetImage"></a>
# **cloudApiControllerGetImage**
> CloudObjectImage cloudApiControllerGetImage(id)

Api Controller Get Image

get image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the image
try {
    val result : CloudObjectImage = apiInstance.cloudApiControllerGetImage(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#cloudApiControllerGetImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#cloudApiControllerGetImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the image | |

### Return type

[**CloudObjectImage**](CloudObjectImage.md)

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

<a id="cloudApiControllerGetImages"></a>
# **cloudApiControllerGetImages**
> CloudObjectImage cloudApiControllerGetImages(pageSize, p)

Api Controller Get Images

get all images

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectImage = apiInstance.cloudApiControllerGetImages(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#cloudApiControllerGetImages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#cloudApiControllerGetImages")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectImage**](CloudObjectImage.md)

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

<a id="cloudApiControllerUpdateImage"></a>
# **cloudApiControllerUpdateImage**
> CloudControllersResponse cloudApiControllerUpdateImage(id, cloudObjectImage)

Api Controller Update Image

update image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the image
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateImage(id, cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#cloudApiControllerUpdateImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#cloudApiControllerUpdateImage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the image | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

<a id="nexusAddImage"></a>
# **nexusAddImage**
> NexusResponse nexusAddImage(cloudObjectImage)

add Image

Add an image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : NexusResponse = apiInstance.nexusAddImage(cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#nexusAddImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#nexusAddImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

<a id="nexusDeleteImage"></a>
# **nexusDeleteImage**
> NexusResponse nexusDeleteImage(cloudObjectImage)

delete Image

Delete an image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : NexusResponse = apiInstance.nexusDeleteImage(cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#nexusDeleteImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#nexusDeleteImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

<a id="nexusGetImage"></a>
# **nexusGetImage**
> CloudObjectImage nexusGetImage(id)

get Image

Get an image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the image
try {
    val result : CloudObjectImage = apiInstance.nexusGetImage(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#nexusGetImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#nexusGetImage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the image | |

### Return type

[**CloudObjectImage**](CloudObjectImage.md)

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

<a id="nexusGetImages"></a>
# **nexusGetImages**
> CloudObjectImage nexusGetImages(pageSize, p)

get Images

Get all images

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectImage = apiInstance.nexusGetImages(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#nexusGetImages")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#nexusGetImages")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectImage**](CloudObjectImage.md)

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

<a id="nexusUpdateImage"></a>
# **nexusUpdateImage**
> NexusResponse nexusUpdateImage(id, cloudObjectImage)

update Image

Update an image

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ImageAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the image
val cloudObjectImage : CloudObjectImage =  // CloudObjectImage | The details of the image
try {
    val result : NexusResponse = apiInstance.nexusUpdateImage(id, cloudObjectImage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImageAPIApi#nexusUpdateImage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImageAPIApi#nexusUpdateImage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the image | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectImage** | [**CloudObjectImage**](CloudObjectImage.md)| The details of the image | |

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

