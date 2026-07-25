# PoliciesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authzAuthzAddPolicy**](PoliciesApi.md#authzAuthzAddPolicy) | **POST** /v1/authz/policies | Add a policy |
| [**authzAuthzListPolicies**](PoliciesApi.md#authzAuthzListPolicies) | **GET** /v1/authz/policies | List policies |
| [**authzAuthzRemovePolicy**](PoliciesApi.md#authzAuthzRemovePolicy) | **DELETE** /v1/authz/policies | Remove a policy |
| [**s3GetBucketPolicy**](PoliciesApi.md#s3GetBucketPolicy) | **GET** /v1/s3/{bucket}?policy | Get bucket policy |
| [**s3PutBucketPolicy**](PoliciesApi.md#s3PutBucketPolicy) | **PUT** /v1/s3/{bucket}?policy | Set bucket policy |


<a id="authzAuthzAddPolicy"></a>
# **authzAuthzAddPolicy**
> AuthzAddPolicyResponse authzAuthzAddPolicy(authzEnforceRequest)

Add a policy

Adds a &#x60;[sub, obj, act]&#x60; rule to the calling org&#39;s policy set. Requires an admin role on the request JWT. Returns &#x60;201&#x60; when the rule was newly added and &#x60;200&#x60; when it already existed. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PoliciesApi()
val authzEnforceRequest : AuthzEnforceRequest =  // AuthzEnforceRequest | 
try {
    val result : AuthzAddPolicyResponse = apiInstance.authzAuthzAddPolicy(authzEnforceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PoliciesApi#authzAuthzAddPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PoliciesApi#authzAuthzAddPolicy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authzEnforceRequest** | [**AuthzEnforceRequest**](AuthzEnforceRequest.md)|  | |

### Return type

[**AuthzAddPolicyResponse**](AuthzAddPolicyResponse.md)

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

<a id="authzAuthzListPolicies"></a>
# **authzAuthzListPolicies**
> AuthzPolicyListResponse authzAuthzListPolicies()

List policies

Returns every policy rule for the calling org as an array of &#x60;[sub, obj, act]&#x60; tuples. Scoped by the gateway-minted &#x60;X-Org-Id&#x60; header. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PoliciesApi()
try {
    val result : AuthzPolicyListResponse = apiInstance.authzAuthzListPolicies()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PoliciesApi#authzAuthzListPolicies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PoliciesApi#authzAuthzListPolicies")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AuthzPolicyListResponse**](AuthzPolicyListResponse.md)

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

<a id="authzAuthzRemovePolicy"></a>
# **authzAuthzRemovePolicy**
> AuthzRemovePolicyResponse authzAuthzRemovePolicy(authzEnforceRequest)

Remove a policy

Removes a &#x60;[sub, obj, act]&#x60; rule from the calling org&#39;s policy set. Requires an admin role on the request JWT. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PoliciesApi()
val authzEnforceRequest : AuthzEnforceRequest =  // AuthzEnforceRequest | 
try {
    val result : AuthzRemovePolicyResponse = apiInstance.authzAuthzRemovePolicy(authzEnforceRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PoliciesApi#authzAuthzRemovePolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PoliciesApi#authzAuthzRemovePolicy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authzEnforceRequest** | [**AuthzEnforceRequest**](AuthzEnforceRequest.md)|  | |

### Return type

[**AuthzRemovePolicyResponse**](AuthzRemovePolicyResponse.md)

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

<a id="s3GetBucketPolicy"></a>
# **s3GetBucketPolicy**
> S3BucketPolicy s3GetBucketPolicy(bucket)

Get bucket policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PoliciesApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : S3BucketPolicy = apiInstance.s3GetBucketPolicy(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PoliciesApi#s3GetBucketPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PoliciesApi#s3GetBucketPolicy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**S3BucketPolicy**](S3BucketPolicy.md)

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

<a id="s3PutBucketPolicy"></a>
# **s3PutBucketPolicy**
> s3PutBucketPolicy(bucket, s3BucketPolicy)

Set bucket policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PoliciesApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val s3BucketPolicy : S3BucketPolicy =  // S3BucketPolicy | 
try {
    apiInstance.s3PutBucketPolicy(bucket, s3BucketPolicy)
} catch (e: ClientException) {
    println("4xx response calling PoliciesApi#s3PutBucketPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PoliciesApi#s3PutBucketPolicy")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3BucketPolicy** | [**S3BucketPolicy**](S3BucketPolicy.md)|  | |

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

