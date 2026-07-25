# CompaniesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**crmCreateCompany**](CompaniesApi.md#crmCreateCompany) | **POST** /v1/crm/companies | Create a company |
| [**crmDeleteCompany**](CompaniesApi.md#crmDeleteCompany) | **DELETE** /v1/crm/companies/{id} | Delete a company (clears dangling contact/opportunity refs) |
| [**crmGetCompany**](CompaniesApi.md#crmGetCompany) | **GET** /v1/crm/companies/{id} | Company detail |
| [**crmListCompanies**](CompaniesApi.md#crmListCompanies) | **GET** /v1/crm/companies | List companies |
| [**crmUpdateCompany**](CompaniesApi.md#crmUpdateCompany) | **PUT** /v1/crm/companies/{id} | Update a company |


<a id="crmCreateCompany"></a>
# **crmCreateCompany**
> CrmCompany crmCreateCompany(crmCompanyInput)

Create a company

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompaniesApi()
val crmCompanyInput : CrmCompanyInput =  // CrmCompanyInput | 
try {
    val result : CrmCompany = apiInstance.crmCreateCompany(crmCompanyInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CompaniesApi#crmCreateCompany")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompaniesApi#crmCreateCompany")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmCompanyInput** | [**CrmCompanyInput**](CrmCompanyInput.md)|  | |

### Return type

[**CrmCompany**](CrmCompany.md)

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

<a id="crmDeleteCompany"></a>
# **crmDeleteCompany**
> crmDeleteCompany(id)

Delete a company (clears dangling contact/opportunity refs)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompaniesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.crmDeleteCompany(id)
} catch (e: ClientException) {
    println("4xx response calling CompaniesApi#crmDeleteCompany")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompaniesApi#crmDeleteCompany")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="crmGetCompany"></a>
# **crmGetCompany**
> CrmCompany crmGetCompany(id)

Company detail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompaniesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : CrmCompany = apiInstance.crmGetCompany(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CompaniesApi#crmGetCompany")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompaniesApi#crmGetCompany")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**CrmCompany**](CrmCompany.md)

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

<a id="crmListCompanies"></a>
# **crmListCompanies**
> CrmListCompanies200Response crmListCompanies(limit)

List companies

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompaniesApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : CrmListCompanies200Response = apiInstance.crmListCompanies(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CompaniesApi#crmListCompanies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompaniesApi#crmListCompanies")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**CrmListCompanies200Response**](CrmListCompanies200Response.md)

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

<a id="crmUpdateCompany"></a>
# **crmUpdateCompany**
> CrmCompany crmUpdateCompany(id, crmCompanyInput)

Update a company

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CompaniesApi()
val id : kotlin.String = id_example // kotlin.String | 
val crmCompanyInput : CrmCompanyInput =  // CrmCompanyInput | 
try {
    val result : CrmCompany = apiInstance.crmUpdateCompany(id, crmCompanyInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CompaniesApi#crmUpdateCompany")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CompaniesApi#crmUpdateCompany")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmCompanyInput** | [**CrmCompanyInput**](CrmCompanyInput.md)|  | |

### Return type

[**CrmCompany**](CrmCompany.md)

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

