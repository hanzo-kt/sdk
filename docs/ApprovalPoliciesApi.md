# ApprovalPoliciesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateChangeApprovalPolicy**](ApprovalPoliciesApi.md#kmsCreateChangeApprovalPolicy) | **POST** /v1/kms/approval-policies/change | Create a secret change approval policy |
| [**kmsListChangeApprovalPolicies**](ApprovalPoliciesApi.md#kmsListChangeApprovalPolicies) | **GET** /v1/kms/approval-policies/change | List secret change approval policies |


<a id="kmsCreateChangeApprovalPolicy"></a>
# **kmsCreateChangeApprovalPolicy**
> KmsCreateChangeApprovalPolicy200Response kmsCreateChangeApprovalPolicy(kmsCreateChangeApprovalPolicyRequest)

Create a secret change approval policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApprovalPoliciesApi()
val kmsCreateChangeApprovalPolicyRequest : KmsCreateChangeApprovalPolicyRequest =  // KmsCreateChangeApprovalPolicyRequest | 
try {
    val result : KmsCreateChangeApprovalPolicy200Response = apiInstance.kmsCreateChangeApprovalPolicy(kmsCreateChangeApprovalPolicyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApprovalPoliciesApi#kmsCreateChangeApprovalPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApprovalPoliciesApi#kmsCreateChangeApprovalPolicy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateChangeApprovalPolicyRequest** | [**KmsCreateChangeApprovalPolicyRequest**](KmsCreateChangeApprovalPolicyRequest.md)|  | |

### Return type

[**KmsCreateChangeApprovalPolicy200Response**](KmsCreateChangeApprovalPolicy200Response.md)

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

<a id="kmsListChangeApprovalPolicies"></a>
# **kmsListChangeApprovalPolicies**
> KmsListChangeApprovalPolicies200Response kmsListChangeApprovalPolicies(workspaceId)

List secret change approval policies

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApprovalPoliciesApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListChangeApprovalPolicies200Response = apiInstance.kmsListChangeApprovalPolicies(workspaceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApprovalPoliciesApi#kmsListChangeApprovalPolicies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApprovalPoliciesApi#kmsListChangeApprovalPolicies")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **workspaceId** | **java.util.UUID**|  | |

### Return type

[**KmsListChangeApprovalPolicies200Response**](KmsListChangeApprovalPolicies200Response.md)

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

