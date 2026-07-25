# AffiliateApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**affiliatesApplyAffiliate**](AffiliateApi.md#affiliatesApplyAffiliate) | **POST** /v1/affiliates/apply | Apply to the affiliate program |
| [**affiliatesAttributeAffiliate**](AffiliateApi.md#affiliatesAttributeAffiliate) | **POST** /v1/affiliates/attribute | Record affiliate attribution |
| [**affiliatesGetMyAffiliate**](AffiliateApi.md#affiliatesGetMyAffiliate) | **GET** /v1/affiliates | Get my affiliate status |


<a id="affiliatesApplyAffiliate"></a>
# **affiliatesApplyAffiliate**
> AffiliatesApplyResponse affiliatesApplyAffiliate(affiliatesApplyRequest)

Apply to the affiliate program

Enrolls the caller org as an affiliate at &#x60;status&#x3D;applied&#x60;. Idempotent (one affiliate per org, first apply wins). A malformed vanity code is refused. Returns &#x60;201&#x60; on first creation, &#x60;200&#x60; if the org was already enrolled. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliateApi()
val affiliatesApplyRequest : AffiliatesApplyRequest =  // AffiliatesApplyRequest | 
try {
    val result : AffiliatesApplyResponse = apiInstance.affiliatesApplyAffiliate(affiliatesApplyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliateApi#affiliatesApplyAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliateApi#affiliatesApplyAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliatesApplyRequest** | [**AffiliatesApplyRequest**](AffiliatesApplyRequest.md)|  | [optional] |

### Return type

[**AffiliatesApplyResponse**](AffiliatesApplyResponse.md)

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

<a id="affiliatesAttributeAffiliate"></a>
# **affiliatesAttributeAffiliate**
> AffiliatesAttributeResponse affiliatesAttributeAffiliate(affiliatesAttributeRequest)

Record affiliate attribution

Records an affiliate↔referred-org edge. The REFERRED org is the validated caller (never client-supplied); the affiliate is resolved from &#x60;code&#x60; (approved affiliates only). Idempotent (one per referred org, first-touch wins); self-attribution is blocked; an unknown code is rejected. Returns &#x60;201&#x60; on first attribution, &#x60;200&#x60; if already attributed. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliateApi()
val affiliatesAttributeRequest : AffiliatesAttributeRequest =  // AffiliatesAttributeRequest | 
try {
    val result : AffiliatesAttributeResponse = apiInstance.affiliatesAttributeAffiliate(affiliatesAttributeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliateApi#affiliatesAttributeAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliateApi#affiliatesAttributeAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliatesAttributeRequest** | [**AffiliatesAttributeRequest**](AffiliatesAttributeRequest.md)|  | |

### Return type

[**AffiliatesAttributeResponse**](AffiliatesAttributeResponse.md)

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

<a id="affiliatesGetMyAffiliate"></a>
# **affiliatesGetMyAffiliate**
> AffiliatesGetMyAffiliate200Response affiliatesGetMyAffiliate()

Get my affiliate status

Returns the caller org&#39;s affiliate dashboard. If the org is not enrolled, returns an honest \&quot;not enrolled\&quot; shape (&#x60;isAffiliate: false&#x60;) so the console can show the apply form. For an APPROVED affiliate it also opportunistically runs the accrual sweep over the org&#39;s own referred orgs (bounded, best-effort), so the dashboard is self-updating. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AffiliateApi()
try {
    val result : AffiliatesGetMyAffiliate200Response = apiInstance.affiliatesGetMyAffiliate()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AffiliateApi#affiliatesGetMyAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AffiliateApi#affiliatesGetMyAffiliate")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AffiliatesGetMyAffiliate200Response**](AffiliatesGetMyAffiliate200Response.md)

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

