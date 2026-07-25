# VideoAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddVideo**](VideoAPIApi.md#cloudApiControllerAddVideo) | **POST** /v1/cloud/add-video | Api Controller Add Video |
| [**cloudApiControllerDeleteVideo**](VideoAPIApi.md#cloudApiControllerDeleteVideo) | **POST** /v1/cloud/delete-video | Api Controller Delete Video |
| [**cloudApiControllerGetGlobalVideos**](VideoAPIApi.md#cloudApiControllerGetGlobalVideos) | **GET** /v1/cloud/get-global-videos | Api Controller Get Global Videos |
| [**cloudApiControllerGetVideo**](VideoAPIApi.md#cloudApiControllerGetVideo) | **GET** /v1/cloud/get-video | Api Controller Get Video |
| [**cloudApiControllerGetVideos**](VideoAPIApi.md#cloudApiControllerGetVideos) | **GET** /v1/cloud/get-videos | Api Controller Get Videos |
| [**cloudApiControllerUpdateVideo**](VideoAPIApi.md#cloudApiControllerUpdateVideo) | **POST** /v1/cloud/update-video | Api Controller Update Video |
| [**cloudApiControllerUploadVideo**](VideoAPIApi.md#cloudApiControllerUploadVideo) | **POST** /v1/cloud/upload-video | Api Controller Upload Video |
| [**nexusAddVideo**](VideoAPIApi.md#nexusAddVideo) | **POST** /v1/nexus/add-video | add Video |
| [**nexusDeleteVideo**](VideoAPIApi.md#nexusDeleteVideo) | **POST** /v1/nexus/delete-video | delete Video |
| [**nexusGetGlobalVideos**](VideoAPIApi.md#nexusGetGlobalVideos) | **GET** /v1/nexus/get-global-videos | get Global Videos |
| [**nexusGetVideo**](VideoAPIApi.md#nexusGetVideo) | **GET** /v1/nexus/get-video | get Video |
| [**nexusGetVideos**](VideoAPIApi.md#nexusGetVideos) | **GET** /v1/nexus/get-videos | get Videos |
| [**nexusUpdateVideo**](VideoAPIApi.md#nexusUpdateVideo) | **POST** /v1/nexus/update-video | update Video |
| [**nexusUploadVideo**](VideoAPIApi.md#nexusUploadVideo) | **POST** /v1/nexus/upload-video | upload Video |


<a id="cloudApiControllerAddVideo"></a>
# **cloudApiControllerAddVideo**
> CloudControllersResponse cloudApiControllerAddVideo(cloudObjectVideo)

Api Controller Add Video

add video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val cloudObjectVideo : CloudObjectVideo =  // CloudObjectVideo | The details of the video
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddVideo(cloudObjectVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerAddVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerAddVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVideo** | [**CloudObjectVideo**](CloudObjectVideo.md)| The details of the video | |

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

<a id="cloudApiControllerDeleteVideo"></a>
# **cloudApiControllerDeleteVideo**
> CloudControllersResponse cloudApiControllerDeleteVideo(cloudObjectVideo)

Api Controller Delete Video

delete video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val cloudObjectVideo : CloudObjectVideo =  // CloudObjectVideo | The details of the video
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteVideo(cloudObjectVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerDeleteVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerDeleteVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVideo** | [**CloudObjectVideo**](CloudObjectVideo.md)| The details of the video | |

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

<a id="cloudApiControllerGetGlobalVideos"></a>
# **cloudApiControllerGetGlobalVideos**
> kotlin.collections.List&lt;CloudObjectVideo&gt; cloudApiControllerGetGlobalVideos()

Api Controller Get Global Videos

get global videos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectVideo> = apiInstance.cloudApiControllerGetGlobalVideos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerGetGlobalVideos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerGetGlobalVideos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectVideo&gt;**](CloudObjectVideo.md)

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

<a id="cloudApiControllerGetVideo"></a>
# **cloudApiControllerGetVideo**
> CloudObjectVideo cloudApiControllerGetVideo(id)

Api Controller Get Video

get video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of video
try {
    val result : CloudObjectVideo = apiInstance.cloudApiControllerGetVideo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerGetVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerGetVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of video | |

### Return type

[**CloudObjectVideo**](CloudObjectVideo.md)

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

<a id="cloudApiControllerGetVideos"></a>
# **cloudApiControllerGetVideos**
> kotlin.collections.List&lt;CloudObjectVideo&gt; cloudApiControllerGetVideos(owner)

Api Controller Get Videos

get videos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of videos
try {
    val result : kotlin.collections.List<CloudObjectVideo> = apiInstance.cloudApiControllerGetVideos(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerGetVideos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerGetVideos")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of videos | |

### Return type

[**kotlin.collections.List&lt;CloudObjectVideo&gt;**](CloudObjectVideo.md)

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

<a id="cloudApiControllerUpdateVideo"></a>
# **cloudApiControllerUpdateVideo**
> CloudControllersResponse cloudApiControllerUpdateVideo(id, cloudObjectVideo)

Api Controller Update Video

update video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the video
val cloudObjectVideo : CloudObjectVideo =  // CloudObjectVideo | The details of the video
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateVideo(id, cloudObjectVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerUpdateVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerUpdateVideo")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the video | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectVideo** | [**CloudObjectVideo**](CloudObjectVideo.md)| The details of the video | |

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

<a id="cloudApiControllerUploadVideo"></a>
# **cloudApiControllerUploadVideo**
> kotlin.String cloudApiControllerUploadVideo(file)

Api Controller Upload Video

upload video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | The video file to upload
try {
    val result : kotlin.String = apiInstance.cloudApiControllerUploadVideo(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#cloudApiControllerUploadVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#cloudApiControllerUploadVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**| The video file to upload | |

### Return type

**kotlin.String**

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

<a id="nexusAddVideo"></a>
# **nexusAddVideo**
> NexusResponse nexusAddVideo(nexusVideo)

add Video

Add a video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val nexusVideo : NexusVideo =  // NexusVideo | The details of the video
try {
    val result : NexusResponse = apiInstance.nexusAddVideo(nexusVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusAddVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusAddVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusVideo** | [**NexusVideo**](NexusVideo.md)| The details of the video | |

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

<a id="nexusDeleteVideo"></a>
# **nexusDeleteVideo**
> NexusResponse nexusDeleteVideo(nexusVideo)

delete Video

Delete a video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val nexusVideo : NexusVideo =  // NexusVideo | The details of the video
try {
    val result : NexusResponse = apiInstance.nexusDeleteVideo(nexusVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusDeleteVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusDeleteVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusVideo** | [**NexusVideo**](NexusVideo.md)| The details of the video | |

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

<a id="nexusGetGlobalVideos"></a>
# **nexusGetGlobalVideos**
> kotlin.collections.List&lt;NexusVideo&gt; nexusGetGlobalVideos()

get Global Videos

Get global videos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
try {
    val result : kotlin.collections.List<NexusVideo> = apiInstance.nexusGetGlobalVideos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusGetGlobalVideos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusGetGlobalVideos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusVideo&gt;**](NexusVideo.md)

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

<a id="nexusGetVideo"></a>
# **nexusGetVideo**
> NexusVideo nexusGetVideo(id)

get Video

Get a video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the video
try {
    val result : NexusVideo = apiInstance.nexusGetVideo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusGetVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusGetVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the video | |

### Return type

[**NexusVideo**](NexusVideo.md)

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

<a id="nexusGetVideos"></a>
# **nexusGetVideos**
> kotlin.collections.List&lt;NexusVideo&gt; nexusGetVideos(owner)

get Videos

Get videos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the videos
try {
    val result : kotlin.collections.List<NexusVideo> = apiInstance.nexusGetVideos(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusGetVideos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusGetVideos")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the videos | |

### Return type

[**kotlin.collections.List&lt;NexusVideo&gt;**](NexusVideo.md)

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

<a id="nexusUpdateVideo"></a>
# **nexusUpdateVideo**
> NexusResponse nexusUpdateVideo(id, nexusVideo)

update Video

Update a video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the video
val nexusVideo : NexusVideo =  // NexusVideo | The details of the video
try {
    val result : NexusResponse = apiInstance.nexusUpdateVideo(id, nexusVideo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusUpdateVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusUpdateVideo")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the video | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusVideo** | [**NexusVideo**](NexusVideo.md)| The details of the video | |

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

<a id="nexusUploadVideo"></a>
# **nexusUploadVideo**
> kotlin.String nexusUploadVideo(file)

upload Video

Upload a video

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VideoAPIApi()
val file : java.io.File = BINARY_DATA_HERE // java.io.File | The video file
try {
    val result : kotlin.String = apiInstance.nexusUploadVideo(file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VideoAPIApi#nexusUploadVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VideoAPIApi#nexusUploadVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**| The video file | |

### Return type

**kotlin.String**

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

