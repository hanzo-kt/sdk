# CheckoutApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceAuthorizeOrder**](CheckoutApi.md#commerceAuthorizeOrder) | **POST** /v1/commerce/order/{orderid}/authorize | Authorize payment for order |
| [**commerceAuthorizePayment**](CheckoutApi.md#commerceAuthorizePayment) | **POST** /v1/commerce/checkout/authorize | Authorize new payment |
| [**commerceAuthorizePaymentForOrder**](CheckoutApi.md#commerceAuthorizePaymentForOrder) | **POST** /v1/commerce/checkout/authorize/{orderid} | Authorize payment for existing order |
| [**commerceCancelOrder**](CheckoutApi.md#commerceCancelOrder) | **POST** /v1/commerce/checkout/cancel/{orderid} | Cancel order |
| [**commerceCaptureOrder**](CheckoutApi.md#commerceCaptureOrder) | **POST** /v1/commerce/order/{orderid}/capture | Capture authorized payment |
| [**commerceCapturePayment**](CheckoutApi.md#commerceCapturePayment) | **POST** /v1/commerce/checkout/capture/{orderid} | Capture authorized payment |
| [**commerceChargeOrder**](CheckoutApi.md#commerceChargeOrder) | **POST** /v1/commerce/order/{orderid}/charge | Authorize and capture payment (single step) |
| [**commerceChargePayment**](CheckoutApi.md#commerceChargePayment) | **POST** /v1/commerce/checkout/charge | Authorize and capture in one step |
| [**commerceConfirmOrder**](CheckoutApi.md#commerceConfirmOrder) | **POST** /v1/commerce/checkout/confirm/{orderid} | Confirm order |
| [**commerceLookupEthereumProxy**](CheckoutApi.md#commerceLookupEthereumProxy) | **GET** /v1/commerce/checkout/ethereum/lookup/{proxyaddress} | Lookup Ethereum proxy address |
| [**commerceRefundOrder**](CheckoutApi.md#commerceRefundOrder) | **POST** /v1/commerce/order/{orderid}/refund | Refund order |
| [**commerceStoreAuthorize**](CheckoutApi.md#commerceStoreAuthorize) | **POST** /v1/commerce/store/{storeid}/checkout/authorize | Authorize payment via store |
| [**commerceStoreCharge**](CheckoutApi.md#commerceStoreCharge) | **POST** /v1/commerce/store/{storeid}/checkout/charge | Charge payment via store |


<a id="commerceAuthorizeOrder"></a>
# **commerceAuthorizeOrder**
> CommerceOrder commerceAuthorizeOrder(orderid, commercePaymentRequest)

Authorize payment for order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commercePaymentRequest : CommercePaymentRequest =  // CommercePaymentRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceAuthorizeOrder(orderid, commercePaymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceAuthorizeOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceAuthorizeOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commercePaymentRequest** | [**CommercePaymentRequest**](CommercePaymentRequest.md)|  | [optional] |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceAuthorizePayment"></a>
# **commerceAuthorizePayment**
> CommerceOrder commerceAuthorizePayment(commerceCheckoutRequest)

Authorize new payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceAuthorizePayment(commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceAuthorizePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceAuthorizePayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCheckoutRequest** | [**CommerceCheckoutRequest**](CommerceCheckoutRequest.md)|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceAuthorizePaymentForOrder"></a>
# **commerceAuthorizePaymentForOrder**
> CommerceOrder commerceAuthorizePaymentForOrder(orderid, commercePaymentRequest)

Authorize payment for existing order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commercePaymentRequest : CommercePaymentRequest =  // CommercePaymentRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceAuthorizePaymentForOrder(orderid, commercePaymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceAuthorizePaymentForOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceAuthorizePaymentForOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commercePaymentRequest** | [**CommercePaymentRequest**](CommercePaymentRequest.md)|  | [optional] |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceCancelOrder"></a>
# **commerceCancelOrder**
> CommerceOrder commerceCancelOrder(orderid)

Cancel order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceCancelOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceCancelOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceCancelOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceCaptureOrder"></a>
# **commerceCaptureOrder**
> CommerceOrder commerceCaptureOrder(orderid)

Capture authorized payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceCaptureOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceCaptureOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceCaptureOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceCapturePayment"></a>
# **commerceCapturePayment**
> CommerceOrder commerceCapturePayment(orderid)

Capture authorized payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceCapturePayment(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceCapturePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceCapturePayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceChargeOrder"></a>
# **commerceChargeOrder**
> CommerceOrder commerceChargeOrder(orderid, commercePaymentRequest)

Authorize and capture payment (single step)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commercePaymentRequest : CommercePaymentRequest =  // CommercePaymentRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceChargeOrder(orderid, commercePaymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceChargeOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceChargeOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commercePaymentRequest** | [**CommercePaymentRequest**](CommercePaymentRequest.md)|  | [optional] |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceChargePayment"></a>
# **commerceChargePayment**
> CommerceOrder commerceChargePayment(commerceCheckoutRequest)

Authorize and capture in one step

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceChargePayment(commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceChargePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceChargePayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCheckoutRequest** | [**CommerceCheckoutRequest**](CommerceCheckoutRequest.md)|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceConfirmOrder"></a>
# **commerceConfirmOrder**
> CommerceOrder commerceConfirmOrder(orderid)

Confirm order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceConfirmOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceConfirmOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceConfirmOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceLookupEthereumProxy"></a>
# **commerceLookupEthereumProxy**
> CommerceLookupEthereumProxy200Response commerceLookupEthereumProxy(proxyaddress)

Lookup Ethereum proxy address

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val proxyaddress : kotlin.String = proxyaddress_example // kotlin.String | 
try {
    val result : CommerceLookupEthereumProxy200Response = apiInstance.commerceLookupEthereumProxy(proxyaddress)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceLookupEthereumProxy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceLookupEthereumProxy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proxyaddress** | **kotlin.String**|  | |

### Return type

[**CommerceLookupEthereumProxy200Response**](CommerceLookupEthereumProxy200Response.md)

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

<a id="commerceRefundOrder"></a>
# **commerceRefundOrder**
> CommerceOrder commerceRefundOrder(orderid, commerceRefundOrderRequest)

Refund order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commerceRefundOrderRequest : CommerceRefundOrderRequest =  // CommerceRefundOrderRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceRefundOrder(orderid, commerceRefundOrderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceRefundOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceRefundOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceRefundOrderRequest** | [**CommerceRefundOrderRequest**](CommerceRefundOrderRequest.md)|  | [optional] |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceStoreAuthorize"></a>
# **commerceStoreAuthorize**
> CommerceOrder commerceStoreAuthorize(storeid, commerceCheckoutRequest)

Authorize payment via store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceStoreAuthorize(storeid, commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceStoreAuthorize")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceStoreAuthorize")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCheckoutRequest** | [**CommerceCheckoutRequest**](CommerceCheckoutRequest.md)|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

<a id="commerceStoreCharge"></a>
# **commerceStoreCharge**
> CommerceOrder commerceStoreCharge(storeid, commerceCheckoutRequest)

Charge payment via store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CheckoutApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceStoreCharge(storeid, commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CheckoutApi#commerceStoreCharge")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CheckoutApi#commerceStoreCharge")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCheckoutRequest** | [**CommerceCheckoutRequest**](CommerceCheckoutRequest.md)|  | |

### Return type

[**CommerceOrder**](CommerceOrder.md)

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

