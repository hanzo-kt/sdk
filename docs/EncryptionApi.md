# EncryptionApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**s3GetBucketEncryption**](EncryptionApi.md#s3GetBucketEncryption) | **GET** /v1/s3/{bucket}?encryption | Get encryption configuration |
| [**s3PutBucketEncryption**](EncryptionApi.md#s3PutBucketEncryption) | **PUT** /v1/s3/{bucket}?encryption | Set encryption configuration |


<a id="s3GetBucketEncryption"></a>
# **s3GetBucketEncryption**
> S3EncryptionConfig s3GetBucketEncryption(bucket)

Get encryption configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EncryptionApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : S3EncryptionConfig = apiInstance.s3GetBucketEncryption(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EncryptionApi#s3GetBucketEncryption")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EncryptionApi#s3GetBucketEncryption")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**S3EncryptionConfig**](S3EncryptionConfig.md)

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

<a id="s3PutBucketEncryption"></a>
# **s3PutBucketEncryption**
> s3PutBucketEncryption(bucket, s3EncryptionConfig)

Set encryption configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EncryptionApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val s3EncryptionConfig : S3EncryptionConfig =  // S3EncryptionConfig | 
try {
    apiInstance.s3PutBucketEncryption(bucket, s3EncryptionConfig)
} catch (e: ClientException) {
    println("4xx response calling EncryptionApi#s3PutBucketEncryption")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EncryptionApi#s3PutBucketEncryption")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3EncryptionConfig** | [**S3EncryptionConfig**](S3EncryptionConfig.md)|  | |

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

