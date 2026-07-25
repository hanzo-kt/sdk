# OrdersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceAuthorizeOrder**](OrdersApi.md#commerceAuthorizeOrder) | **POST** /v1/commerce/order/{orderid}/authorize | Authorize payment for order |
| [**commerceCaptureOrder**](OrdersApi.md#commerceCaptureOrder) | **POST** /v1/commerce/order/{orderid}/capture | Capture authorized payment |
| [**commerceChargeOrder**](OrdersApi.md#commerceChargeOrder) | **POST** /v1/commerce/order/{orderid}/charge | Authorize and capture payment (single step) |
| [**commerceCreateOrder**](OrdersApi.md#commerceCreateOrder) | **POST** /v1/commerce/order | Create order |
| [**commerceDeleteOrder**](OrdersApi.md#commerceDeleteOrder) | **DELETE** /v1/commerce/order/{orderid} | Delete order |
| [**commerceGetOrder**](OrdersApi.md#commerceGetOrder) | **GET** /v1/commerce/order/{orderid} | Get order |
| [**commerceGetOrderPayments**](OrdersApi.md#commerceGetOrderPayments) | **GET** /v1/commerce/order/{orderid}/payments | Get order payments |
| [**commerceGetOrderReturns**](OrdersApi.md#commerceGetOrderReturns) | **GET** /v1/commerce/order/{orderid}/returns | Get order returns |
| [**commerceGetOrderStatus**](OrdersApi.md#commerceGetOrderStatus) | **GET** /v1/commerce/order/{orderid}/status | Get order status |
| [**commerceListOrders**](OrdersApi.md#commerceListOrders) | **GET** /v1/commerce/order | List orders |
| [**commercePatchOrder**](OrdersApi.md#commercePatchOrder) | **PATCH** /v1/commerce/order/{orderid} | Partially update order |
| [**commerceRefundOrder**](OrdersApi.md#commerceRefundOrder) | **POST** /v1/commerce/order/{orderid}/refund | Refund order |
| [**commerceSendFulfillmentConfirmation**](OrdersApi.md#commerceSendFulfillmentConfirmation) | **GET** /v1/commerce/order/{orderid}/sendfulfillmentconfirmation | Send fulfillment confirmation email |
| [**commerceSendOrderConfirmation**](OrdersApi.md#commerceSendOrderConfirmation) | **GET** /v1/commerce/order/{orderid}/sendorderconfirmation | Send order confirmation email |
| [**commerceSendRefundConfirmation**](OrdersApi.md#commerceSendRefundConfirmation) | **GET** /v1/commerce/order/{orderid}/sendrefundconfirmation | Send refund confirmation email |
| [**commerceUpdateOrder**](OrdersApi.md#commerceUpdateOrder) | **PUT** /v1/commerce/order/{orderid} | Update order |


<a id="commerceAuthorizeOrder"></a>
# **commerceAuthorizeOrder**
> CommerceOrder commerceAuthorizeOrder(orderid, commercePaymentRequest)

Authorize payment for order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commercePaymentRequest : CommercePaymentRequest =  // CommercePaymentRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceAuthorizeOrder(orderid, commercePaymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceAuthorizeOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceAuthorizeOrder")
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

<a id="commerceCaptureOrder"></a>
# **commerceCaptureOrder**
> CommerceOrder commerceCaptureOrder(orderid)

Capture authorized payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceCaptureOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceCaptureOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceCaptureOrder")
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

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commercePaymentRequest : CommercePaymentRequest =  // CommercePaymentRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceChargeOrder(orderid, commercePaymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceChargeOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceChargeOrder")
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

<a id="commerceCreateOrder"></a>
# **commerceCreateOrder**
> CommerceOrder commerceCreateOrder(commerceOrder)

Create order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val commerceOrder : CommerceOrder =  // CommerceOrder | 
try {
    val result : CommerceOrder = apiInstance.commerceCreateOrder(commerceOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceCreateOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceCreateOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceOrder** | [**CommerceOrder**](CommerceOrder.md)|  | |

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

<a id="commerceDeleteOrder"></a>
# **commerceDeleteOrder**
> commerceDeleteOrder(orderid)

Delete order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    apiInstance.commerceDeleteOrder(orderid)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceDeleteOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceDeleteOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

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

<a id="commerceGetOrder"></a>
# **commerceGetOrder**
> CommerceOrder commerceGetOrder(orderid)

Get order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceOrder = apiInstance.commerceGetOrder(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceGetOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceGetOrder")
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

<a id="commerceGetOrderPayments"></a>
# **commerceGetOrderPayments**
> kotlin.collections.List&lt;CommercePayment&gt; commerceGetOrderPayments(orderid)

Get order payments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommercePayment> = apiInstance.commerceGetOrderPayments(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceGetOrderPayments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceGetOrderPayments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommercePayment&gt;**](CommercePayment.md)

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

<a id="commerceGetOrderReturns"></a>
# **commerceGetOrderReturns**
> kotlin.collections.List&lt;CommerceReturn&gt; commerceGetOrderReturns(orderid)

Get order returns

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceReturn> = apiInstance.commerceGetOrderReturns(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceGetOrderReturns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceGetOrderReturns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceReturn&gt;**](CommerceReturn.md)

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

<a id="commerceGetOrderStatus"></a>
# **commerceGetOrderStatus**
> CommerceGetOrderStatus200Response commerceGetOrderStatus(orderid)

Get order status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : CommerceGetOrderStatus200Response = apiInstance.commerceGetOrderStatus(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceGetOrderStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceGetOrderStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

### Return type

[**CommerceGetOrderStatus200Response**](CommerceGetOrderStatus200Response.md)

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

<a id="commerceListOrders"></a>
# **commerceListOrders**
> CommercePaginatedOrders commerceListOrders(page, display, sort, q)

List orders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
val sort : kotlin.String = sort_example // kotlin.String | Sort field (prefix with - for descending)
val q : kotlin.String = q_example // kotlin.String | Search query
try {
    val result : CommercePaginatedOrders = apiInstance.commerceListOrders(page, display, sort, q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceListOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceListOrders")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**| Page number (1-indexed) | [optional] [default to 1] |
| **display** | **kotlin.Int**| Number of items per page | [optional] [default to 20] |
| **sort** | **kotlin.String**| Sort field (prefix with - for descending) | [optional] [default to &quot;-UpdatedAt&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**| Search query | [optional] |

### Return type

[**CommercePaginatedOrders**](CommercePaginatedOrders.md)

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

<a id="commercePatchOrder"></a>
# **commercePatchOrder**
> CommerceOrder commercePatchOrder(orderid, commerceOrder)

Partially update order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commerceOrder : CommerceOrder =  // CommerceOrder | 
try {
    val result : CommerceOrder = apiInstance.commercePatchOrder(orderid, commerceOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commercePatchOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commercePatchOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceOrder** | [**CommerceOrder**](CommerceOrder.md)|  | |

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

<a id="commerceRefundOrder"></a>
# **commerceRefundOrder**
> CommerceOrder commerceRefundOrder(orderid, commerceRefundOrderRequest)

Refund order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commerceRefundOrderRequest : CommerceRefundOrderRequest =  // CommerceRefundOrderRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceRefundOrder(orderid, commerceRefundOrderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceRefundOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceRefundOrder")
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

<a id="commerceSendFulfillmentConfirmation"></a>
# **commerceSendFulfillmentConfirmation**
> kotlin.Any commerceSendFulfillmentConfirmation(orderid)

Send fulfillment confirmation email

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceSendFulfillmentConfirmation(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceSendFulfillmentConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceSendFulfillmentConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

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

<a id="commerceSendOrderConfirmation"></a>
# **commerceSendOrderConfirmation**
> kotlin.Any commerceSendOrderConfirmation(orderid)

Send order confirmation email

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceSendOrderConfirmation(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceSendOrderConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceSendOrderConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

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

<a id="commerceSendRefundConfirmation"></a>
# **commerceSendRefundConfirmation**
> kotlin.Any commerceSendRefundConfirmation(orderid)

Send refund confirmation email

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceSendRefundConfirmation(orderid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceSendRefundConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceSendRefundConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderid** | **kotlin.String**|  | |

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

<a id="commerceUpdateOrder"></a>
# **commerceUpdateOrder**
> CommerceOrder commerceUpdateOrder(orderid, commerceOrder)

Update order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrdersApi()
val orderid : kotlin.String = orderid_example // kotlin.String | 
val commerceOrder : CommerceOrder =  // CommerceOrder | 
try {
    val result : CommerceOrder = apiInstance.commerceUpdateOrder(orderid, commerceOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrdersApi#commerceUpdateOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrdersApi#commerceUpdateOrder")
    e.printStackTrace()
}
```

### Parameters
| **orderid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceOrder** | [**CommerceOrder**](CommerceOrder.md)|  | |

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

