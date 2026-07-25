# CustomersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminCustomerDetail**](CustomersApi.md#adminAdminCustomerDetail) | **GET** /v1/admin/customers/{org} | One customer&#39;s detail |
| [**adminAdminGrantCredit**](CustomersApi.md#adminAdminGrantCredit) | **POST** /v1/admin/customers/{org}/credit | Grant credit (commerce deposit) |
| [**adminAdminListCustomers**](CustomersApi.md#adminAdminListCustomers) | **GET** /v1/admin/customers | Fleet customer list |
| [**adminAdminReactivateCustomer**](CustomersApi.md#adminAdminReactivateCustomer) | **POST** /v1/admin/customers/{org}/reactivate | Reactivate a customer (IAM isForbidden&#x3D;false) |
| [**adminAdminSuspendCustomer**](CustomersApi.md#adminAdminSuspendCustomer) | **POST** /v1/admin/customers/{org}/suspend | Suspend a customer (IAM isForbidden&#x3D;true) |


<a id="adminAdminCustomerDetail"></a>
# **adminAdminCustomerDetail**
> AdminAdminCustomerDetail200Response adminAdminCustomerDetail(org)

One customer&#39;s detail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomersApi()
val org : kotlin.String = org_example // kotlin.String | 
try {
    val result : AdminAdminCustomerDetail200Response = apiInstance.adminAdminCustomerDetail(org)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#adminAdminCustomerDetail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#adminAdminCustomerDetail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **org** | **kotlin.String**|  | |

### Return type

[**AdminAdminCustomerDetail200Response**](AdminAdminCustomerDetail200Response.md)

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

<a id="adminAdminGrantCredit"></a>
# **adminAdminGrantCredit**
> AdminAdminGrantCredit200Response adminAdminGrantCredit(org, adminCreditRequest)

Grant credit (commerce deposit)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomersApi()
val org : kotlin.String = org_example // kotlin.String | 
val adminCreditRequest : AdminCreditRequest =  // AdminCreditRequest | 
try {
    val result : AdminAdminGrantCredit200Response = apiInstance.adminAdminGrantCredit(org, adminCreditRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#adminAdminGrantCredit")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#adminAdminGrantCredit")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **adminCreditRequest** | [**AdminCreditRequest**](AdminCreditRequest.md)|  | |

### Return type

[**AdminAdminGrantCredit200Response**](AdminAdminGrantCredit200Response.md)

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

<a id="adminAdminListCustomers"></a>
# **adminAdminListCustomers**
> AdminAdminListCustomers200Response adminAdminListCustomers()

Fleet customer list

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomersApi()
try {
    val result : AdminAdminListCustomers200Response = apiInstance.adminAdminListCustomers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#adminAdminListCustomers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#adminAdminListCustomers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminListCustomers200Response**](AdminAdminListCustomers200Response.md)

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

<a id="adminAdminReactivateCustomer"></a>
# **adminAdminReactivateCustomer**
> AdminAdminReactivateCustomer200Response adminAdminReactivateCustomer(org)

Reactivate a customer (IAM isForbidden&#x3D;false)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomersApi()
val org : kotlin.String = org_example // kotlin.String | 
try {
    val result : AdminAdminReactivateCustomer200Response = apiInstance.adminAdminReactivateCustomer(org)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#adminAdminReactivateCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#adminAdminReactivateCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **org** | **kotlin.String**|  | |

### Return type

[**AdminAdminReactivateCustomer200Response**](AdminAdminReactivateCustomer200Response.md)

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

<a id="adminAdminSuspendCustomer"></a>
# **adminAdminSuspendCustomer**
> AdminAdminReactivateCustomer200Response adminAdminSuspendCustomer(org)

Suspend a customer (IAM isForbidden&#x3D;true)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CustomersApi()
val org : kotlin.String = org_example // kotlin.String | 
try {
    val result : AdminAdminReactivateCustomer200Response = apiInstance.adminAdminSuspendCustomer(org)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomersApi#adminAdminSuspendCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomersApi#adminAdminSuspendCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **org** | **kotlin.String**|  | |

### Return type

[**AdminAdminReactivateCustomer200Response**](AdminAdminReactivateCustomer200Response.md)

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

