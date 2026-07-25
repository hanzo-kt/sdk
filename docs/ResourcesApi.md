# ResourcesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddResource**](ResourcesApi.md#iamApiControllerAddResource) | **POST** /v1/iam/resources | Api Controller Add Resource |
| [**iamApiControllerDeleteResource**](ResourcesApi.md#iamApiControllerDeleteResource) | **DELETE** /v1/iam/resources/{id} | Api Controller Delete Resource |
| [**iamApiControllerGetResource**](ResourcesApi.md#iamApiControllerGetResource) | **GET** /v1/iam/resources/{id} | Api Controller Get Resource |
| [**iamApiControllerGetResources**](ResourcesApi.md#iamApiControllerGetResources) | **GET** /v1/iam/resources | Api Controller Get Resources |
| [**iamApiControllerUpdateResource**](ResourcesApi.md#iamApiControllerUpdateResource) | **PUT** /v1/iam/resources/{id} | Api Controller Update Resource |
| [**iamApiControllerUploadResource**](ResourcesApi.md#iamApiControllerUploadResource) | **POST** /v1/iam/resources/upload | Api Controller Upload Resource |


<a id="iamApiControllerAddResource"></a>
# **iamApiControllerAddResource**
> IamControllersResponse iamApiControllerAddResource(iamObjectResource)

Api Controller Add Resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val iamObjectResource : IamObjectResource =  // IamObjectResource | Resource object
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddResource(iamObjectResource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerAddResource")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerAddResource")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectResource** | [**IamObjectResource**](IamObjectResource.md)| Resource object | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteResource"></a>
# **iamApiControllerDeleteResource**
> IamControllersResponse iamApiControllerDeleteResource(id, iamObjectResource)

Api Controller Delete Resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectResource : IamObjectResource =  // IamObjectResource | Resource object
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteResource(id, iamObjectResource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerDeleteResource")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerDeleteResource")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectResource** | [**IamObjectResource**](IamObjectResource.md)| Resource object | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetResource"></a>
# **iamApiControllerGetResource**
> IamObjectResource iamApiControllerGetResource(id)

Api Controller Get Resource

get resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of resource
try {
    val result : IamObjectResource = apiInstance.iamApiControllerGetResource(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerGetResource")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerGetResource")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of resource | |

### Return type

[**IamObjectResource**](IamObjectResource.md)

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

<a id="iamApiControllerGetResources"></a>
# **iamApiControllerGetResources**
> kotlin.collections.List&lt;IamObjectResource&gt; iamApiControllerGetResources(owner, user, pageSize, p, `field`, `value`, sortField, sortOrder)

Api Controller Get Resources

get resources

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val owner : kotlin.String = owner_example // kotlin.String | Owner
val user : kotlin.String = user_example // kotlin.String | User
val pageSize : kotlin.Int = 56 // kotlin.Int | Page Size
val p : kotlin.Int = 56 // kotlin.Int | Page Number
val `field` : kotlin.String = `field`_example // kotlin.String | Field
val `value` : kotlin.String = `value`_example // kotlin.String | Value
val sortField : kotlin.String = sortField_example // kotlin.String | Sort Field
val sortOrder : kotlin.String = sortOrder_example // kotlin.String | Sort Order
try {
    val result : kotlin.collections.List<IamObjectResource> = apiInstance.iamApiControllerGetResources(owner, user, pageSize, p, `field`, `value`, sortField, sortOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerGetResources")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerGetResources")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| Owner | |
| **user** | **kotlin.String**| User | |
| **pageSize** | **kotlin.Int**| Page Size | [optional] |
| **p** | **kotlin.Int**| Page Number | [optional] |
| **&#x60;field&#x60;** | **kotlin.String**| Field | [optional] |
| **&#x60;value&#x60;** | **kotlin.String**| Value | [optional] |
| **sortField** | **kotlin.String**| Sort Field | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sortOrder** | **kotlin.String**| Sort Order | [optional] |

### Return type

[**kotlin.collections.List&lt;IamObjectResource&gt;**](IamObjectResource.md)

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

<a id="iamApiControllerUpdateResource"></a>
# **iamApiControllerUpdateResource**
> IamControllersResponse iamApiControllerUpdateResource(id, iamObjectResource)

Api Controller Update Resource

get resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of resource
val iamObjectResource : IamObjectResource =  // IamObjectResource | The resource object
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateResource(id, iamObjectResource)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerUpdateResource")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerUpdateResource")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of resource | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectResource** | [**IamObjectResource**](IamObjectResource.md)| The resource object | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUploadResource"></a>
# **iamApiControllerUploadResource**
> IamObjectResource iamApiControllerUploadResource(owner, user, application, fullFilePath, file, tag, parent, createdTime, description)

Api Controller Upload Resource

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ResourcesApi()
val owner : kotlin.String = owner_example // kotlin.String | Owner
val user : kotlin.String = user_example // kotlin.String | User
val application : kotlin.String = application_example // kotlin.String | Application
val fullFilePath : kotlin.String = fullFilePath_example // kotlin.String | Full File Path
val file : java.io.File = BINARY_DATA_HERE // java.io.File | Resource file
val tag : kotlin.String = tag_example // kotlin.String | Tag
val parent : kotlin.String = parent_example // kotlin.String | Parent
val createdTime : kotlin.String = createdTime_example // kotlin.String | Created Time
val description : kotlin.String = description_example // kotlin.String | Description
try {
    val result : IamObjectResource = apiInstance.iamApiControllerUploadResource(owner, user, application, fullFilePath, file, tag, parent, createdTime, description)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ResourcesApi#iamApiControllerUploadResource")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ResourcesApi#iamApiControllerUploadResource")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| Owner | |
| **user** | **kotlin.String**| User | |
| **application** | **kotlin.String**| Application | |
| **fullFilePath** | **kotlin.String**| Full File Path | |
| **file** | **java.io.File**| Resource file | |
| **tag** | **kotlin.String**| Tag | [optional] |
| **parent** | **kotlin.String**| Parent | [optional] |
| **createdTime** | **kotlin.String**| Created Time | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **description** | **kotlin.String**| Description | [optional] |

### Return type

[**IamObjectResource**](IamObjectResource.md)

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

