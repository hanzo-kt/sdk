# ObjectsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**s3DeleteObject**](ObjectsApi.md#s3DeleteObject) | **DELETE** /v1/s3/{bucket}/{key} | Delete an object |
| [**s3GetObject**](ObjectsApi.md#s3GetObject) | **GET** /v1/s3/{bucket}/{key} | Download an object |
| [**s3HeadObject**](ObjectsApi.md#s3HeadObject) | **HEAD** /v1/s3/{bucket}/{key} | Get object metadata |
| [**s3ListObjectsV2**](ObjectsApi.md#s3ListObjectsV2) | **GET** /v1/s3/{bucket} | List objects in bucket |
| [**s3PutObject**](ObjectsApi.md#s3PutObject) | **PUT** /v1/s3/{bucket}/{key} | Upload an object |


<a id="s3DeleteObject"></a>
# **s3DeleteObject**
> s3DeleteObject(bucket, key, versionId)

Delete an object

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val versionId : kotlin.String = versionId_example // kotlin.String | Specific version to delete
try {
    apiInstance.s3DeleteObject(bucket, key, versionId)
} catch (e: ClientException) {
    println("4xx response calling ObjectsApi#s3DeleteObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectsApi#s3DeleteObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **versionId** | **kotlin.String**| Specific version to delete | [optional] |

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
 - **Accept**: Not defined

<a id="s3GetObject"></a>
# **s3GetObject**
> java.io.File s3GetObject(bucket, key, versionId, range)

Download an object

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val versionId : kotlin.String = versionId_example // kotlin.String | Specific version to retrieve
val range : kotlin.String = range_example // kotlin.String | Byte range (e.g. bytes=0-1023)
try {
    val result : java.io.File = apiInstance.s3GetObject(bucket, key, versionId, range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectsApi#s3GetObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectsApi#s3GetObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| **versionId** | **kotlin.String**| Specific version to retrieve | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**| Byte range (e.g. bytes&#x3D;0-1023) | [optional] |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream

<a id="s3HeadObject"></a>
# **s3HeadObject**
> s3HeadObject(bucket, key)

Get object metadata

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    apiInstance.s3HeadObject(bucket, key)
} catch (e: ClientException) {
    println("4xx response calling ObjectsApi#s3HeadObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectsApi#s3HeadObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="s3ListObjectsV2"></a>
# **s3ListObjectsV2**
> S3ListObjectsV2200Response s3ListObjectsV2(bucket, prefix, delimiter, maxKeys, continuationToken)

List objects in bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val prefix : kotlin.String = prefix_example // kotlin.String | Filter by key prefix
val delimiter : kotlin.String = delimiter_example // kotlin.String | Grouping delimiter (e.g. /)
val maxKeys : kotlin.Int = 56 // kotlin.Int | 
val continuationToken : kotlin.String = continuationToken_example // kotlin.String | Pagination token from previous response
try {
    val result : S3ListObjectsV2200Response = apiInstance.s3ListObjectsV2(bucket, prefix, delimiter, maxKeys, continuationToken)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ObjectsApi#s3ListObjectsV2")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectsApi#s3ListObjectsV2")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **prefix** | **kotlin.String**| Filter by key prefix | [optional] |
| **delimiter** | **kotlin.String**| Grouping delimiter (e.g. /) | [optional] |
| **maxKeys** | **kotlin.Int**|  | [optional] [default to 1000] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **continuationToken** | **kotlin.String**| Pagination token from previous response | [optional] |

### Return type

[**S3ListObjectsV2200Response**](S3ListObjectsV2200Response.md)

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

<a id="s3PutObject"></a>
# **s3PutObject**
> s3PutObject(bucket, key, body, contentType, xAmzServerSideEncryption)

Upload an object

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ObjectsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
val contentType : kotlin.String = contentType_example // kotlin.String | 
val xAmzServerSideEncryption : kotlin.String = xAmzServerSideEncryption_example // kotlin.String | Server-side encryption algorithm
try {
    apiInstance.s3PutObject(bucket, key, body, contentType, xAmzServerSideEncryption)
} catch (e: ClientException) {
    println("4xx response calling ObjectsApi#s3PutObject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ObjectsApi#s3PutObject")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| **body** | **java.io.File**|  | |
| **contentType** | **kotlin.String**|  | [optional] [default to &quot;application/octet-stream&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **xAmzServerSideEncryption** | **kotlin.String**| Server-side encryption algorithm | [optional] [enum: AES256, aws:kms] |

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

 - **Content-Type**: application/octet-stream
 - **Accept**: Not defined

