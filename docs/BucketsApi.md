# BucketsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**s3CreateBucket**](BucketsApi.md#s3CreateBucket) | **PUT** /v1/s3/{bucket} | Create a bucket |
| [**s3DeleteBucket**](BucketsApi.md#s3DeleteBucket) | **DELETE** /v1/s3/{bucket} | Delete a bucket |
| [**s3ListBuckets**](BucketsApi.md#s3ListBuckets) | **GET** /v1/s3/ | List all buckets |


<a id="s3CreateBucket"></a>
# **s3CreateBucket**
> s3CreateBucket(bucket)

Create a bucket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BucketsApi()
val bucket : kotlin.String = my-models // kotlin.String | 
try {
    apiInstance.s3CreateBucket(bucket)
} catch (e: ClientException) {
    println("4xx response calling BucketsApi#s3CreateBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BucketsApi#s3CreateBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

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
 - **Accept**: application/json

<a id="s3DeleteBucket"></a>
# **s3DeleteBucket**
> s3DeleteBucket(bucket)

Delete a bucket

Bucket must be empty before deletion.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BucketsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    apiInstance.s3DeleteBucket(bucket)
} catch (e: ClientException) {
    println("4xx response calling BucketsApi#s3DeleteBucket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BucketsApi#s3DeleteBucket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

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

<a id="s3ListBuckets"></a>
# **s3ListBuckets**
> S3ListBuckets200Response s3ListBuckets()

List all buckets

Returns a list of all buckets owned by the authenticated user.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BucketsApi()
try {
    val result : S3ListBuckets200Response = apiInstance.s3ListBuckets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BucketsApi#s3ListBuckets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BucketsApi#s3ListBuckets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**S3ListBuckets200Response**](S3ListBuckets200Response.md)

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

