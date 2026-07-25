# PaymentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddOrder**](PaymentsApi.md#iamApiControllerAddOrder) | **POST** /v1/iam/orders | Api Controller Add Order |
| [**iamApiControllerAddPayment**](PaymentsApi.md#iamApiControllerAddPayment) | **POST** /v1/iam/payments | Api Controller Add Payment |
| [**iamApiControllerAddPlan**](PaymentsApi.md#iamApiControllerAddPlan) | **POST** /v1/iam/plans | Api Controller Add Plan |
| [**iamApiControllerAddPricing**](PaymentsApi.md#iamApiControllerAddPricing) | **POST** /v1/iam/pricings | Api Controller Add Pricing |
| [**iamApiControllerAddProduct**](PaymentsApi.md#iamApiControllerAddProduct) | **POST** /v1/iam/products | Api Controller Add Product |
| [**iamApiControllerAddSubscription**](PaymentsApi.md#iamApiControllerAddSubscription) | **POST** /v1/iam/subscriptions | Api Controller Add Subscription |
| [**iamApiControllerAddTransaction**](PaymentsApi.md#iamApiControllerAddTransaction) | **POST** /v1/iam/transactions | Api Controller Add Transaction |
| [**iamApiControllerCancelOrder**](PaymentsApi.md#iamApiControllerCancelOrder) | **POST** /v1/iam/orders/cancel | Api Controller Cancel Order |
| [**iamApiControllerDeleteOrder**](PaymentsApi.md#iamApiControllerDeleteOrder) | **DELETE** /v1/iam/orders/{id} | Api Controller Delete Order |
| [**iamApiControllerDeletePayment**](PaymentsApi.md#iamApiControllerDeletePayment) | **DELETE** /v1/iam/payments/{id} | Api Controller Delete Payment |
| [**iamApiControllerDeletePlan**](PaymentsApi.md#iamApiControllerDeletePlan) | **DELETE** /v1/iam/plans/{id} | Api Controller Delete Plan |
| [**iamApiControllerDeletePricing**](PaymentsApi.md#iamApiControllerDeletePricing) | **DELETE** /v1/iam/pricings/{id} | Api Controller Delete Pricing |
| [**iamApiControllerDeleteProduct**](PaymentsApi.md#iamApiControllerDeleteProduct) | **DELETE** /v1/iam/products/{id} | Api Controller Delete Product |
| [**iamApiControllerDeleteSubscription**](PaymentsApi.md#iamApiControllerDeleteSubscription) | **DELETE** /v1/iam/subscriptions/{id} | Api Controller Delete Subscription |
| [**iamApiControllerDeleteTransaction**](PaymentsApi.md#iamApiControllerDeleteTransaction) | **DELETE** /v1/iam/transactions/{id} | Api Controller Delete Transaction |
| [**iamApiControllerGetOrder**](PaymentsApi.md#iamApiControllerGetOrder) | **GET** /v1/iam/orders/{id} | Api Controller Get Order |
| [**iamApiControllerGetOrders**](PaymentsApi.md#iamApiControllerGetOrders) | **GET** /v1/iam/orders | Api Controller Get Orders |
| [**iamApiControllerGetPlan**](PaymentsApi.md#iamApiControllerGetPlan) | **GET** /v1/iam/plans/{id} | Api Controller Get Plan |
| [**iamApiControllerGetPlans**](PaymentsApi.md#iamApiControllerGetPlans) | **GET** /v1/iam/plans | Api Controller Get Plans |
| [**iamApiControllerGetPricing**](PaymentsApi.md#iamApiControllerGetPricing) | **GET** /v1/iam/pricings/{id} | Api Controller Get Pricing |
| [**iamApiControllerGetPricings**](PaymentsApi.md#iamApiControllerGetPricings) | **GET** /v1/iam/pricings | Api Controller Get Pricings |
| [**iamApiControllerGetProduct**](PaymentsApi.md#iamApiControllerGetProduct) | **GET** /v1/iam/products/{id} | Api Controller Get Product |
| [**iamApiControllerGetProducts**](PaymentsApi.md#iamApiControllerGetProducts) | **GET** /v1/iam/products | Api Controller Get Products |
| [**iamApiControllerGetSubscription**](PaymentsApi.md#iamApiControllerGetSubscription) | **GET** /v1/iam/subscriptions/{id} | Api Controller Get Subscription |
| [**iamApiControllerGetSubscriptions**](PaymentsApi.md#iamApiControllerGetSubscriptions) | **GET** /v1/iam/subscriptions | Api Controller Get Subscriptions |
| [**iamApiControllerGetTransaction**](PaymentsApi.md#iamApiControllerGetTransaction) | **GET** /v1/iam/transactions/{id} | Api Controller Get Transaction |
| [**iamApiControllerGetTransactions**](PaymentsApi.md#iamApiControllerGetTransactions) | **GET** /v1/iam/transactions | Api Controller Get Transactions |
| [**iamApiControllerGetUserOrders**](PaymentsApi.md#iamApiControllerGetUserOrders) | **GET** /v1/iam/user-orders | Api Controller Get User Orders |
| [**iamApiControllerInvoicePayment**](PaymentsApi.md#iamApiControllerInvoicePayment) | **POST** /v1/iam/invoice-payment | Api Controller Invoice Payment |
| [**iamApiControllerNotifyPayment**](PaymentsApi.md#iamApiControllerNotifyPayment) | **POST** /v1/iam/payments/notify | Api Controller Notify Payment |
| [**iamApiControllerPayOrder**](PaymentsApi.md#iamApiControllerPayOrder) | **POST** /v1/iam/pay-order | Api Controller Pay Order |
| [**iamApiControllerPlaceOrder**](PaymentsApi.md#iamApiControllerPlaceOrder) | **POST** /v1/iam/place-order | Api Controller Place Order |
| [**iamApiControllerUpdateOrder**](PaymentsApi.md#iamApiControllerUpdateOrder) | **PUT** /v1/iam/orders/{id} | Api Controller Update Order |
| [**iamApiControllerUpdatePayment**](PaymentsApi.md#iamApiControllerUpdatePayment) | **PUT** /v1/iam/payments/{id} | Api Controller Update Payment |
| [**iamApiControllerUpdatePlan**](PaymentsApi.md#iamApiControllerUpdatePlan) | **PUT** /v1/iam/plans/{id} | Api Controller Update Plan |
| [**iamApiControllerUpdatePricing**](PaymentsApi.md#iamApiControllerUpdatePricing) | **PUT** /v1/iam/pricings/{id} | Api Controller Update Pricing |
| [**iamApiControllerUpdateProduct**](PaymentsApi.md#iamApiControllerUpdateProduct) | **PUT** /v1/iam/products/{id} | Api Controller Update Product |
| [**iamApiControllerUpdateSubscription**](PaymentsApi.md#iamApiControllerUpdateSubscription) | **PUT** /v1/iam/subscriptions/{id} | Api Controller Update Subscription |
| [**iamApiControllerUpdateTransaction**](PaymentsApi.md#iamApiControllerUpdateTransaction) | **PUT** /v1/iam/transactions/{id} | Api Controller Update Transaction |


<a id="iamApiControllerAddOrder"></a>
# **iamApiControllerAddOrder**
> IamControllersResponse iamApiControllerAddOrder(iamObjectOrder)

Api Controller Add Order

add order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectOrder : IamObjectOrder =  // IamObjectOrder | The details of the order
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddOrder(iamObjectOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrder** | [**IamObjectOrder**](IamObjectOrder.md)| The details of the order | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddPayment"></a>
# **iamApiControllerAddPayment**
> IamControllersResponse iamApiControllerAddPayment(iamObjectPayment)

Api Controller Add Payment

add payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectPayment : IamObjectPayment =  // IamObjectPayment | The details of the payment
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddPayment(iamObjectPayment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddPayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddPayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPayment** | [**IamObjectPayment**](IamObjectPayment.md)| The details of the payment | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddPlan"></a>
# **iamApiControllerAddPlan**
> IamControllersResponse iamApiControllerAddPlan(iamObjectPlan)

Api Controller Add Plan

add plan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectPlan : IamObjectPlan =  // IamObjectPlan | The details of the plan
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddPlan(iamObjectPlan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddPlan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddPlan")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPlan** | [**IamObjectPlan**](IamObjectPlan.md)| The details of the plan | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddPricing"></a>
# **iamApiControllerAddPricing**
> IamControllersResponse iamApiControllerAddPricing(iamObjectPricing)

Api Controller Add Pricing

add pricing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectPricing : IamObjectPricing =  // IamObjectPricing | The details of the pricing
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddPricing(iamObjectPricing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddPricing")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPricing** | [**IamObjectPricing**](IamObjectPricing.md)| The details of the pricing | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddProduct"></a>
# **iamApiControllerAddProduct**
> IamControllersResponse iamApiControllerAddProduct(iamObjectProduct)

Api Controller Add Product

add product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectProduct : IamObjectProduct =  // IamObjectProduct | The details of the product
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddProduct(iamObjectProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProduct** | [**IamObjectProduct**](IamObjectProduct.md)| The details of the product | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddSubscription"></a>
# **iamApiControllerAddSubscription**
> IamControllersResponse iamApiControllerAddSubscription(iamObjectSubscription)

Api Controller Add Subscription

add subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectSubscription : IamObjectSubscription =  // IamObjectSubscription | The details of the subscription
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddSubscription(iamObjectSubscription)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSubscription** | [**IamObjectSubscription**](IamObjectSubscription.md)| The details of the subscription | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerAddTransaction"></a>
# **iamApiControllerAddTransaction**
> IamControllersResponse iamApiControllerAddTransaction(iamObjectTransaction, dryRun)

Api Controller Add Transaction

add transaction

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectTransaction : IamObjectTransaction =  // IamObjectTransaction | The details of the transaction
val dryRun : kotlin.String = dryRun_example // kotlin.String | Dry run mode: set to 'true' or '1' to validate without committing
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddTransaction(iamObjectTransaction, dryRun)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerAddTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerAddTransaction")
    e.printStackTrace()
}
```

### Parameters
| **iamObjectTransaction** | [**IamObjectTransaction**](IamObjectTransaction.md)| The details of the transaction | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dryRun** | **kotlin.String**| Dry run mode: set to &#39;true&#39; or &#39;1&#39; to validate without committing | [optional] |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerCancelOrder"></a>
# **iamApiControllerCancelOrder**
> IamControllersResponse iamApiControllerCancelOrder(id)

Api Controller Cancel Order

cancel an order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the order
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerCancelOrder(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerCancelOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerCancelOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the order | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteOrder"></a>
# **iamApiControllerDeleteOrder**
> IamControllersResponse iamApiControllerDeleteOrder(id, iamObjectOrder)

Api Controller Delete Order

delete order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectOrder : IamObjectOrder =  // IamObjectOrder | The details of the order
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteOrder(id, iamObjectOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeleteOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeleteOrder")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrder** | [**IamObjectOrder**](IamObjectOrder.md)| The details of the order | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeletePayment"></a>
# **iamApiControllerDeletePayment**
> IamControllersResponse iamApiControllerDeletePayment(id, iamObjectPayment)

Api Controller Delete Payment

delete payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectPayment : IamObjectPayment =  // IamObjectPayment | The details of the payment
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeletePayment(id, iamObjectPayment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeletePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeletePayment")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPayment** | [**IamObjectPayment**](IamObjectPayment.md)| The details of the payment | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeletePlan"></a>
# **iamApiControllerDeletePlan**
> IamControllersResponse iamApiControllerDeletePlan(id, iamObjectPlan)

Api Controller Delete Plan

delete plan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectPlan : IamObjectPlan =  // IamObjectPlan | The details of the plan
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeletePlan(id, iamObjectPlan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeletePlan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeletePlan")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPlan** | [**IamObjectPlan**](IamObjectPlan.md)| The details of the plan | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeletePricing"></a>
# **iamApiControllerDeletePricing**
> IamControllersResponse iamApiControllerDeletePricing(id, iamObjectPricing)

Api Controller Delete Pricing

delete pricing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectPricing : IamObjectPricing =  // IamObjectPricing | The details of the pricing
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeletePricing(id, iamObjectPricing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeletePricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeletePricing")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPricing** | [**IamObjectPricing**](IamObjectPricing.md)| The details of the pricing | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteProduct"></a>
# **iamApiControllerDeleteProduct**
> IamControllersResponse iamApiControllerDeleteProduct(id, iamObjectProduct)

Api Controller Delete Product

delete product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectProduct : IamObjectProduct =  // IamObjectProduct | The details of the product
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteProduct(id, iamObjectProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeleteProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeleteProduct")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProduct** | [**IamObjectProduct**](IamObjectProduct.md)| The details of the product | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteSubscription"></a>
# **iamApiControllerDeleteSubscription**
> IamControllersResponse iamApiControllerDeleteSubscription(id, iamObjectSubscription)

Api Controller Delete Subscription

delete subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectSubscription : IamObjectSubscription =  // IamObjectSubscription | The details of the subscription
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteSubscription(id, iamObjectSubscription)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeleteSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeleteSubscription")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSubscription** | [**IamObjectSubscription**](IamObjectSubscription.md)| The details of the subscription | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteTransaction"></a>
# **iamApiControllerDeleteTransaction**
> IamControllersResponse iamApiControllerDeleteTransaction(id, iamObjectTransaction)

Api Controller Delete Transaction

delete transaction

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectTransaction : IamObjectTransaction =  // IamObjectTransaction | The details of the transaction
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteTransaction(id, iamObjectTransaction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerDeleteTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerDeleteTransaction")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTransaction** | [**IamObjectTransaction**](IamObjectTransaction.md)| The details of the transaction | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetOrder"></a>
# **iamApiControllerGetOrder**
> IamObjectOrder iamApiControllerGetOrder(id)

Api Controller Get Order

get order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the order
try {
    val result : IamObjectOrder = apiInstance.iamApiControllerGetOrder(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the order | |

### Return type

[**IamObjectOrder**](IamObjectOrder.md)

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

<a id="iamApiControllerGetOrders"></a>
# **iamApiControllerGetOrders**
> kotlin.collections.List&lt;IamObjectOrder&gt; iamApiControllerGetOrders(owner)

Api Controller Get Orders

get orders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of orders
try {
    val result : kotlin.collections.List<IamObjectOrder> = apiInstance.iamApiControllerGetOrders(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of orders | |

### Return type

[**kotlin.collections.List&lt;IamObjectOrder&gt;**](IamObjectOrder.md)

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

<a id="iamApiControllerGetPlan"></a>
# **iamApiControllerGetPlan**
> IamObjectPlan iamApiControllerGetPlan(id, includeOption)

Api Controller Get Plan

get plan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the plan
val includeOption : kotlin.Boolean = true // kotlin.Boolean | Should include plan's option
try {
    val result : IamObjectPlan = apiInstance.iamApiControllerGetPlan(id, includeOption)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetPlan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetPlan")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the plan | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **includeOption** | **kotlin.Boolean**| Should include plan&#39;s option | [optional] |

### Return type

[**IamObjectPlan**](IamObjectPlan.md)

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

<a id="iamApiControllerGetPlans"></a>
# **iamApiControllerGetPlans**
> kotlin.collections.List&lt;IamObjectPlan&gt; iamApiControllerGetPlans(owner)

Api Controller Get Plans

get plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of plans
try {
    val result : kotlin.collections.List<IamObjectPlan> = apiInstance.iamApiControllerGetPlans(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetPlans")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of plans | |

### Return type

[**kotlin.collections.List&lt;IamObjectPlan&gt;**](IamObjectPlan.md)

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

<a id="iamApiControllerGetPricing"></a>
# **iamApiControllerGetPricing**
> IamObjectPricing iamApiControllerGetPricing(id)

Api Controller Get Pricing

get pricing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the pricing
try {
    val result : IamObjectPricing = apiInstance.iamApiControllerGetPricing(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetPricing")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the pricing | |

### Return type

[**IamObjectPricing**](IamObjectPricing.md)

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

<a id="iamApiControllerGetPricings"></a>
# **iamApiControllerGetPricings**
> kotlin.collections.List&lt;IamObjectPricing&gt; iamApiControllerGetPricings(owner)

Api Controller Get Pricings

get pricings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of pricings
try {
    val result : kotlin.collections.List<IamObjectPricing> = apiInstance.iamApiControllerGetPricings(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetPricings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetPricings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of pricings | |

### Return type

[**kotlin.collections.List&lt;IamObjectPricing&gt;**](IamObjectPricing.md)

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

<a id="iamApiControllerGetProduct"></a>
# **iamApiControllerGetProduct**
> IamObjectProduct iamApiControllerGetProduct(id)

Api Controller Get Product

get product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the product
try {
    val result : IamObjectProduct = apiInstance.iamApiControllerGetProduct(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the product | |

### Return type

[**IamObjectProduct**](IamObjectProduct.md)

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

<a id="iamApiControllerGetProducts"></a>
# **iamApiControllerGetProducts**
> kotlin.collections.List&lt;IamObjectProduct&gt; iamApiControllerGetProducts(owner)

Api Controller Get Products

get products

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of products
try {
    val result : kotlin.collections.List<IamObjectProduct> = apiInstance.iamApiControllerGetProducts(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetProducts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of products | |

### Return type

[**kotlin.collections.List&lt;IamObjectProduct&gt;**](IamObjectProduct.md)

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

<a id="iamApiControllerGetSubscription"></a>
# **iamApiControllerGetSubscription**
> IamObjectSubscription iamApiControllerGetSubscription(id)

Api Controller Get Subscription

get subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the subscription
try {
    val result : IamObjectSubscription = apiInstance.iamApiControllerGetSubscription(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the subscription | |

### Return type

[**IamObjectSubscription**](IamObjectSubscription.md)

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

<a id="iamApiControllerGetSubscriptions"></a>
# **iamApiControllerGetSubscriptions**
> kotlin.collections.List&lt;IamObjectSubscription&gt; iamApiControllerGetSubscriptions(owner)

Api Controller Get Subscriptions

get subscriptions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of subscriptions
try {
    val result : kotlin.collections.List<IamObjectSubscription> = apiInstance.iamApiControllerGetSubscriptions(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetSubscriptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetSubscriptions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of subscriptions | |

### Return type

[**kotlin.collections.List&lt;IamObjectSubscription&gt;**](IamObjectSubscription.md)

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

<a id="iamApiControllerGetTransaction"></a>
# **iamApiControllerGetTransaction**
> IamObjectTransaction iamApiControllerGetTransaction(id)

Api Controller Get Transaction

get transaction

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the transaction
try {
    val result : IamObjectTransaction = apiInstance.iamApiControllerGetTransaction(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetTransaction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the transaction | |

### Return type

[**IamObjectTransaction**](IamObjectTransaction.md)

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

<a id="iamApiControllerGetTransactions"></a>
# **iamApiControllerGetTransactions**
> kotlin.collections.List&lt;IamObjectTransaction&gt; iamApiControllerGetTransactions(owner)

Api Controller Get Transactions

get transactions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of transactions
try {
    val result : kotlin.collections.List<IamObjectTransaction> = apiInstance.iamApiControllerGetTransactions(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetTransactions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetTransactions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of transactions | |

### Return type

[**kotlin.collections.List&lt;IamObjectTransaction&gt;**](IamObjectTransaction.md)

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

<a id="iamApiControllerGetUserOrders"></a>
# **iamApiControllerGetUserOrders**
> kotlin.collections.List&lt;IamObjectOrder&gt; iamApiControllerGetUserOrders(owner, user)

Api Controller Get User Orders

get orders for a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of orders
val user : kotlin.String = user_example // kotlin.String | The username of the user
try {
    val result : kotlin.collections.List<IamObjectOrder> = apiInstance.iamApiControllerGetUserOrders(owner, user)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerGetUserOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerGetUserOrders")
    e.printStackTrace()
}
```

### Parameters
| **owner** | **kotlin.String**| The owner of orders | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user** | **kotlin.String**| The username of the user | |

### Return type

[**kotlin.collections.List&lt;IamObjectOrder&gt;**](IamObjectOrder.md)

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

<a id="iamApiControllerInvoicePayment"></a>
# **iamApiControllerInvoicePayment**
> IamControllersResponse iamApiControllerInvoicePayment(id)

Api Controller Invoice Payment

invoice payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the payment
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerInvoicePayment(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerInvoicePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerInvoicePayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the payment | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerNotifyPayment"></a>
# **iamApiControllerNotifyPayment**
> IamControllersResponse iamApiControllerNotifyPayment(iamObjectPayment)

Api Controller Notify Payment

notify payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val iamObjectPayment : IamObjectPayment =  // IamObjectPayment | The details of the payment
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerNotifyPayment(iamObjectPayment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerNotifyPayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerNotifyPayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPayment** | [**IamObjectPayment**](IamObjectPayment.md)| The details of the payment | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerPayOrder"></a>
# **iamApiControllerPayOrder**
> IamControllersResponse iamApiControllerPayOrder(id, providerName)

Api Controller Pay Order

pay an existing order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the order
val providerName : kotlin.String = providerName_example // kotlin.String | The name of the provider
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerPayOrder(id, providerName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerPayOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerPayOrder")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the order | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **providerName** | **kotlin.String**| The name of the provider | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerPlaceOrder"></a>
# **iamApiControllerPlaceOrder**
> IamObjectOrder iamApiControllerPlaceOrder(productId, pricingName, planName, customPrice, userName)

Api Controller Place Order

place an order for a product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val productId : kotlin.String = productId_example // kotlin.String | The id ( owner/name ) of the product
val pricingName : kotlin.String = pricingName_example // kotlin.String | The name of the pricing (for subscription)
val planName : kotlin.String = planName_example // kotlin.String | The name of the plan (for subscription)
val customPrice : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Custom price for recharge products
val userName : kotlin.String = userName_example // kotlin.String | The username to place order for (admin only)
try {
    val result : IamObjectOrder = apiInstance.iamApiControllerPlaceOrder(productId, pricingName, planName, customPrice, userName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerPlaceOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerPlaceOrder")
    e.printStackTrace()
}
```

### Parameters
| **productId** | **kotlin.String**| The id ( owner/name ) of the product | |
| **pricingName** | **kotlin.String**| The name of the pricing (for subscription) | [optional] |
| **planName** | **kotlin.String**| The name of the plan (for subscription) | [optional] |
| **customPrice** | **java.math.BigDecimal**| Custom price for recharge products | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userName** | **kotlin.String**| The username to place order for (admin only) | [optional] |

### Return type

[**IamObjectOrder**](IamObjectOrder.md)

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

<a id="iamApiControllerUpdateOrder"></a>
# **iamApiControllerUpdateOrder**
> IamControllersResponse iamApiControllerUpdateOrder(id, iamObjectOrder)

Api Controller Update Order

update order

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the order
val iamObjectOrder : IamObjectOrder =  // IamObjectOrder | The details of the order
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateOrder(id, iamObjectOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdateOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdateOrder")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the order | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrder** | [**IamObjectOrder**](IamObjectOrder.md)| The details of the order | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdatePayment"></a>
# **iamApiControllerUpdatePayment**
> IamControllersResponse iamApiControllerUpdatePayment(id, iamObjectPayment)

Api Controller Update Payment

update payment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the payment
val iamObjectPayment : IamObjectPayment =  // IamObjectPayment | The details of the payment
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdatePayment(id, iamObjectPayment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdatePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdatePayment")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the payment | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPayment** | [**IamObjectPayment**](IamObjectPayment.md)| The details of the payment | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdatePlan"></a>
# **iamApiControllerUpdatePlan**
> IamControllersResponse iamApiControllerUpdatePlan(id, iamObjectPlan)

Api Controller Update Plan

update plan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the plan
val iamObjectPlan : IamObjectPlan =  // IamObjectPlan | The details of the plan
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdatePlan(id, iamObjectPlan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdatePlan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdatePlan")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the plan | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPlan** | [**IamObjectPlan**](IamObjectPlan.md)| The details of the plan | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdatePricing"></a>
# **iamApiControllerUpdatePricing**
> IamControllersResponse iamApiControllerUpdatePricing(id, iamObjectPricing)

Api Controller Update Pricing

update pricing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the pricing
val iamObjectPricing : IamObjectPricing =  // IamObjectPricing | The details of the pricing
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdatePricing(id, iamObjectPricing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdatePricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdatePricing")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the pricing | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPricing** | [**IamObjectPricing**](IamObjectPricing.md)| The details of the pricing | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdateProduct"></a>
# **iamApiControllerUpdateProduct**
> IamControllersResponse iamApiControllerUpdateProduct(id, iamObjectProduct)

Api Controller Update Product

update product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the product
val iamObjectProduct : IamObjectProduct =  // IamObjectProduct | The details of the product
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateProduct(id, iamObjectProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdateProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdateProduct")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the product | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectProduct** | [**IamObjectProduct**](IamObjectProduct.md)| The details of the product | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdateSubscription"></a>
# **iamApiControllerUpdateSubscription**
> IamControllersResponse iamApiControllerUpdateSubscription(id, iamObjectSubscription)

Api Controller Update Subscription

update subscription

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the subscription
val iamObjectSubscription : IamObjectSubscription =  // IamObjectSubscription | The details of the subscription
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateSubscription(id, iamObjectSubscription)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdateSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdateSubscription")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the subscription | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSubscription** | [**IamObjectSubscription**](IamObjectSubscription.md)| The details of the subscription | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerUpdateTransaction"></a>
# **iamApiControllerUpdateTransaction**
> IamControllersResponse iamApiControllerUpdateTransaction(id, iamObjectTransaction)

Api Controller Update Transaction

update transaction

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PaymentsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the transaction
val iamObjectTransaction : IamObjectTransaction =  // IamObjectTransaction | The details of the transaction
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateTransaction(id, iamObjectTransaction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentsApi#iamApiControllerUpdateTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentsApi#iamApiControllerUpdateTransaction")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the transaction | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTransaction** | [**IamObjectTransaction**](IamObjectTransaction.md)| The details of the transaction | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

