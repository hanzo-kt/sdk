# SubscriptionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCancelSubscription**](SubscriptionsApi.md#commerceCancelSubscription) | **DELETE** /v1/commerce/subscribe/{subscriptionid} | Cancel subscription |
| [**commerceCreateSubscription**](SubscriptionsApi.md#commerceCreateSubscription) | **POST** /v1/commerce/subscribe | Create subscription |
| [**commerceGetSubscription**](SubscriptionsApi.md#commerceGetSubscription) | **GET** /v1/commerce/subscribe/{subscriptionid} | Get subscription |
| [**commerceUpdateSubscription**](SubscriptionsApi.md#commerceUpdateSubscription) | **PATCH** /v1/commerce/subscribe/{subscriptionid} | Update subscription |
| [**pricingListBlockchainPlans**](SubscriptionsApi.md#pricingListBlockchainPlans) | **GET** /v1/pricing/blockchain | Blockchain / RPC plans |
| [**pricingListPlans**](SubscriptionsApi.md#pricingListPlans) | **GET** /v1/pricing/plans | Subscription plans |
| [**pricingListSubscriptions**](SubscriptionsApi.md#pricingListSubscriptions) | **GET** /v1/pricing/subscriptions | Subscription plans |


<a id="commerceCancelSubscription"></a>
# **commerceCancelSubscription**
> CommerceSubscription commerceCancelSubscription(subscriptionid)

Cancel subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
val subscriptionid : kotlin.String = subscriptionid_example // kotlin.String | 
try {
    val result : CommerceSubscription = apiInstance.commerceCancelSubscription(subscriptionid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#commerceCancelSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#commerceCancelSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscriptionid** | **kotlin.String**|  | |

### Return type

[**CommerceSubscription**](CommerceSubscription.md)

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

<a id="commerceCreateSubscription"></a>
# **commerceCreateSubscription**
> CommerceSubscription commerceCreateSubscription(commerceSubscriptionRequest)

Create subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
val commerceSubscriptionRequest : CommerceSubscriptionRequest =  // CommerceSubscriptionRequest | 
try {
    val result : CommerceSubscription = apiInstance.commerceCreateSubscription(commerceSubscriptionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#commerceCreateSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#commerceCreateSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSubscriptionRequest** | [**CommerceSubscriptionRequest**](CommerceSubscriptionRequest.md)|  | |

### Return type

[**CommerceSubscription**](CommerceSubscription.md)

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

<a id="commerceGetSubscription"></a>
# **commerceGetSubscription**
> CommerceSubscription commerceGetSubscription(subscriptionid)

Get subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
val subscriptionid : kotlin.String = subscriptionid_example // kotlin.String | 
try {
    val result : CommerceSubscription = apiInstance.commerceGetSubscription(subscriptionid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#commerceGetSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#commerceGetSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscriptionid** | **kotlin.String**|  | |

### Return type

[**CommerceSubscription**](CommerceSubscription.md)

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

<a id="commerceUpdateSubscription"></a>
# **commerceUpdateSubscription**
> CommerceSubscription commerceUpdateSubscription(subscriptionid, commerceSubscription)

Update subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
val subscriptionid : kotlin.String = subscriptionid_example // kotlin.String | 
val commerceSubscription : CommerceSubscription =  // CommerceSubscription | 
try {
    val result : CommerceSubscription = apiInstance.commerceUpdateSubscription(subscriptionid, commerceSubscription)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#commerceUpdateSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#commerceUpdateSubscription")
    e.printStackTrace()
}
```

### Parameters
| **subscriptionid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSubscription** | [**CommerceSubscription**](CommerceSubscription.md)|  | |

### Return type

[**CommerceSubscription**](CommerceSubscription.md)

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

<a id="pricingListBlockchainPlans"></a>
# **pricingListBlockchainPlans**
> PricingListBlockchainPlans200Response pricingListBlockchainPlans()

Blockchain / RPC plans

Returns blockchain node and RPC access plans.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
try {
    val result : PricingListBlockchainPlans200Response = apiInstance.pricingListBlockchainPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#pricingListBlockchainPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#pricingListBlockchainPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingListBlockchainPlans200Response**](PricingListBlockchainPlans200Response.md)

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

<a id="pricingListPlans"></a>
# **pricingListPlans**
> PricingSubscriptionPlansResponse pricingListPlans()

Subscription plans

Returns platform subscription plans across the personal, team, world, social, and enterprise categories (e.g. Developer, Pro, Max, Team, World Free/Pro/Team/Enterprise). Alias for /v1/pricing/subscriptions. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
try {
    val result : PricingSubscriptionPlansResponse = apiInstance.pricingListPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#pricingListPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#pricingListPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingSubscriptionPlansResponse**](PricingSubscriptionPlansResponse.md)

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

<a id="pricingListSubscriptions"></a>
# **pricingListSubscriptions**
> PricingSubscriptionPlansResponse pricingListSubscriptions()

Subscription plans

Returns platform subscription plans with pricing, features, rate limits, and revenue sharing details. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubscriptionsApi()
try {
    val result : PricingSubscriptionPlansResponse = apiInstance.pricingListSubscriptions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubscriptionsApi#pricingListSubscriptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubscriptionsApi#pricingListSubscriptions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingSubscriptionPlansResponse**](PricingSubscriptionPlansResponse.md)

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

