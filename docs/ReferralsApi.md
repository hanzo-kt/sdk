# ReferralsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**referralsClaimReferral**](ReferralsApi.md#referralsClaimReferral) | **POST** /v1/referrals/claim | Claim a referral from a ?ref code |
| [**referralsGetMyReferrals**](ReferralsApi.md#referralsGetMyReferrals) | **GET** /v1/referrals | Get my referral code, link, and referrals |


<a id="referralsClaimReferral"></a>
# **referralsClaimReferral**
> ReferralsClaimResponse referralsClaimReferral(referralsClaimRequest)

Claim a referral from a ?ref code

Records a referral. The REFEREE is the validated caller (never client- supplied); the referrer is resolved from the code. Idempotent (one per referee, first-touch wins); self-referral is blocked; an unknown code is rejected. Returns 201 when a new referral was created, 200 when it already existed. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReferralsApi()
val referralsClaimRequest : ReferralsClaimRequest =  // ReferralsClaimRequest | 
try {
    val result : ReferralsClaimResponse = apiInstance.referralsClaimReferral(referralsClaimRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReferralsApi#referralsClaimReferral")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReferralsApi#referralsClaimReferral")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **referralsClaimRequest** | [**ReferralsClaimRequest**](ReferralsClaimRequest.md)|  | |

### Return type

[**ReferralsClaimResponse**](ReferralsClaimResponse.md)

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

<a id="referralsGetMyReferrals"></a>
# **referralsGetMyReferrals**
> ReferralsMyReferralsResponse referralsGetMyReferrals()

Get my referral code, link, and referrals

Returns the caller org&#39;s stable referral code and link, the referrals they have made (with per-referral status and credit earned), a status tally, and the total credit earned. Opportunistically runs the qualify check for the caller&#39;s own pending referees, so the page is self-updating. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReferralsApi()
try {
    val result : ReferralsMyReferralsResponse = apiInstance.referralsGetMyReferrals()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReferralsApi#referralsGetMyReferrals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReferralsApi#referralsGetMyReferrals")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ReferralsMyReferralsResponse**](ReferralsMyReferralsResponse.md)

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

