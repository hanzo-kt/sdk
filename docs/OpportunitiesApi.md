# OpportunitiesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**crmCreateOpportunity**](OpportunitiesApi.md#crmCreateOpportunity) | **POST** /v1/crm/opportunities | Create an opportunity |
| [**crmDeleteOpportunity**](OpportunitiesApi.md#crmDeleteOpportunity) | **DELETE** /v1/crm/opportunities/{id} | Delete an opportunity |
| [**crmGetOpportunity**](OpportunitiesApi.md#crmGetOpportunity) | **GET** /v1/crm/opportunities/{id} | Opportunity detail |
| [**crmListOpportunities**](OpportunitiesApi.md#crmListOpportunities) | **GET** /v1/crm/opportunities | List opportunities |
| [**crmUpdateOpportunity**](OpportunitiesApi.md#crmUpdateOpportunity) | **PUT** /v1/crm/opportunities/{id} | Update an opportunity |


<a id="crmCreateOpportunity"></a>
# **crmCreateOpportunity**
> CrmOpportunity crmCreateOpportunity(crmOpportunityInput)

Create an opportunity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpportunitiesApi()
val crmOpportunityInput : CrmOpportunityInput =  // CrmOpportunityInput | 
try {
    val result : CrmOpportunity = apiInstance.crmCreateOpportunity(crmOpportunityInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpportunitiesApi#crmCreateOpportunity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpportunitiesApi#crmCreateOpportunity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmOpportunityInput** | [**CrmOpportunityInput**](CrmOpportunityInput.md)|  | |

### Return type

[**CrmOpportunity**](CrmOpportunity.md)

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

<a id="crmDeleteOpportunity"></a>
# **crmDeleteOpportunity**
> crmDeleteOpportunity(id)

Delete an opportunity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpportunitiesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.crmDeleteOpportunity(id)
} catch (e: ClientException) {
    println("4xx response calling OpportunitiesApi#crmDeleteOpportunity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpportunitiesApi#crmDeleteOpportunity")
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

<a id="crmGetOpportunity"></a>
# **crmGetOpportunity**
> CrmOpportunity crmGetOpportunity(id)

Opportunity detail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpportunitiesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : CrmOpportunity = apiInstance.crmGetOpportunity(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpportunitiesApi#crmGetOpportunity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpportunitiesApi#crmGetOpportunity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**CrmOpportunity**](CrmOpportunity.md)

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

<a id="crmListOpportunities"></a>
# **crmListOpportunities**
> CrmListOpportunities200Response crmListOpportunities(stage, limit)

List opportunities

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpportunitiesApi()
val stage : CrmStage =  // CrmStage | Filter to one pipeline stage
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : CrmListOpportunities200Response = apiInstance.crmListOpportunities(stage, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpportunitiesApi#crmListOpportunities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpportunitiesApi#crmListOpportunities")
    e.printStackTrace()
}
```

### Parameters
| **stage** | [**CrmStage**](.md)| Filter to one pipeline stage | [optional] [enum: NEW, SCREENING, MEETING, PROPOSAL, CUSTOMER] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**CrmListOpportunities200Response**](CrmListOpportunities200Response.md)

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

<a id="crmUpdateOpportunity"></a>
# **crmUpdateOpportunity**
> CrmOpportunity crmUpdateOpportunity(id, crmOpportunityInput)

Update an opportunity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OpportunitiesApi()
val id : kotlin.String = id_example // kotlin.String | 
val crmOpportunityInput : CrmOpportunityInput =  // CrmOpportunityInput | 
try {
    val result : CrmOpportunity = apiInstance.crmUpdateOpportunity(id, crmOpportunityInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OpportunitiesApi#crmUpdateOpportunity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OpportunitiesApi#crmUpdateOpportunity")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmOpportunityInput** | [**CrmOpportunityInput**](CrmOpportunityInput.md)|  | |

### Return type

[**CrmOpportunity**](CrmOpportunity.md)

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

