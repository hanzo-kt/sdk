# VersioningApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**s3GetBucketVersioning**](VersioningApi.md#s3GetBucketVersioning) | **GET** /v1/s3/{bucket}?versioning | Get versioning status |
| [**s3PutBucketVersioning**](VersioningApi.md#s3PutBucketVersioning) | **PUT** /v1/s3/{bucket}?versioning | Set versioning status |


<a id="s3GetBucketVersioning"></a>
# **s3GetBucketVersioning**
> S3VersioningConfig s3GetBucketVersioning(bucket)

Get versioning status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VersioningApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : S3VersioningConfig = apiInstance.s3GetBucketVersioning(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VersioningApi#s3GetBucketVersioning")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VersioningApi#s3GetBucketVersioning")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**S3VersioningConfig**](S3VersioningConfig.md)

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

<a id="s3PutBucketVersioning"></a>
# **s3PutBucketVersioning**
> s3PutBucketVersioning(bucket, s3VersioningConfig)

Set versioning status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = VersioningApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val s3VersioningConfig : S3VersioningConfig =  // S3VersioningConfig | 
try {
    apiInstance.s3PutBucketVersioning(bucket, s3VersioningConfig)
} catch (e: ClientException) {
    println("4xx response calling VersioningApi#s3PutBucketVersioning")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VersioningApi#s3PutBucketVersioning")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3VersioningConfig** | [**S3VersioningConfig**](S3VersioningConfig.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

