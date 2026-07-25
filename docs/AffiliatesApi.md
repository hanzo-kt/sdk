# AffiliatesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceConnectAffiliate**](AffiliatesApi.md#commerceConnectAffiliate) | **GET** /v1/commerce/affiliate/{affiliateid}/connect | Connect affiliate |
| [**commerceCreateAffiliate**](AffiliatesApi.md#commerceCreateAffiliate) | **POST** /v1/commerce/affiliate | Create affiliate |
| [**commerceGetAffiliate**](AffiliatesApi.md#commerceGetAffiliate) | **GET** /v1/commerce/affiliate/{affiliateid} | Get affiliate |
| [**commerceListAffiliates**](AffiliatesApi.md#commerceListAffiliates) | **GET** /v1/commerce/affiliate | List affiliates |


<a id="commerceConnectAffiliate"></a>
# **commerceConnectAffiliate**
> kotlin.Any commerceConnectAffiliate(affiliateid)

Connect affiliate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliatesApi()
val affiliateid : kotlin.String = affiliateid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceConnectAffiliate(affiliateid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliatesApi#commerceConnectAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliatesApi#commerceConnectAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliateid** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="commerceCreateAffiliate"></a>
# **commerceCreateAffiliate**
> CommerceAffiliate commerceCreateAffiliate(commerceAffiliate)

Create affiliate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliatesApi()
val commerceAffiliate : CommerceAffiliate =  // CommerceAffiliate | 
try {
    val result : CommerceAffiliate = apiInstance.commerceCreateAffiliate(commerceAffiliate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliatesApi#commerceCreateAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliatesApi#commerceCreateAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceAffiliate** | [**CommerceAffiliate**](CommerceAffiliate.md)|  | |

### Return type

[**CommerceAffiliate**](CommerceAffiliate.md)

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

<a id="commerceGetAffiliate"></a>
# **commerceGetAffiliate**
> CommerceAffiliate commerceGetAffiliate(affiliateid)

Get affiliate

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliatesApi()
val affiliateid : kotlin.String = affiliateid_example // kotlin.String | 
try {
    val result : CommerceAffiliate = apiInstance.commerceGetAffiliate(affiliateid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliatesApi#commerceGetAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliatesApi#commerceGetAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliateid** | **kotlin.String**|  | |

### Return type

[**CommerceAffiliate**](CommerceAffiliate.md)

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

<a id="commerceListAffiliates"></a>
# **commerceListAffiliates**
> CommercePaginatedAffiliates commerceListAffiliates(page, display)

List affiliates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliatesApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
try {
    val result : CommercePaginatedAffiliates = apiInstance.commerceListAffiliates(page, display)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliatesApi#commerceListAffiliates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliatesApi#commerceListAffiliates")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**| Page number (1-indexed) | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **display** | **kotlin.Int**| Number of items per page | [optional] [default to 20] |

### Return type

[**CommercePaginatedAffiliates**](CommercePaginatedAffiliates.md)

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

