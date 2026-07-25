# LifecycleApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**s3GetBucketLifecycle**](LifecycleApi.md#s3GetBucketLifecycle) | **GET** /v1/s3/{bucket}?lifecycle | Get lifecycle rules |
| [**s3PutBucketLifecycle**](LifecycleApi.md#s3PutBucketLifecycle) | **PUT** /v1/s3/{bucket}?lifecycle | Set lifecycle rules |


<a id="s3GetBucketLifecycle"></a>
# **s3GetBucketLifecycle**
> S3GetBucketLifecycle200Response s3GetBucketLifecycle(bucket)

Get lifecycle rules

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LifecycleApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : S3GetBucketLifecycle200Response = apiInstance.s3GetBucketLifecycle(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LifecycleApi#s3GetBucketLifecycle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LifecycleApi#s3GetBucketLifecycle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**S3GetBucketLifecycle200Response**](S3GetBucketLifecycle200Response.md)

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

<a id="s3PutBucketLifecycle"></a>
# **s3PutBucketLifecycle**
> s3PutBucketLifecycle(bucket, s3GetBucketLifecycle200Response)

Set lifecycle rules

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LifecycleApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val s3GetBucketLifecycle200Response : S3GetBucketLifecycle200Response =  // S3GetBucketLifecycle200Response | 
try {
    apiInstance.s3PutBucketLifecycle(bucket, s3GetBucketLifecycle200Response)
} catch (e: ClientException) {
    println("4xx response calling LifecycleApi#s3PutBucketLifecycle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LifecycleApi#s3PutBucketLifecycle")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3GetBucketLifecycle200Response** | [**S3GetBucketLifecycle200Response**](S3GetBucketLifecycle200Response.md)|  | |

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

