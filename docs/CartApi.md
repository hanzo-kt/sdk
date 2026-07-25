# CartApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateCart**](CartApi.md#commerceCreateCart) | **POST** /v1/commerce/cart | Create cart |
| [**commerceDeleteCart**](CartApi.md#commerceDeleteCart) | **DELETE** /v1/commerce/cart/{cartid} | Delete cart |
| [**commerceDiscardCart**](CartApi.md#commerceDiscardCart) | **POST** /v1/commerce/cart/{cartid}/discard | Discard cart |
| [**commerceGetCart**](CartApi.md#commerceGetCart) | **GET** /v1/commerce/cart/{cartid} | Get cart |
| [**commerceListCarts**](CartApi.md#commerceListCarts) | **GET** /v1/commerce/cart | List carts |
| [**commercePatchCart**](CartApi.md#commercePatchCart) | **PATCH** /v1/commerce/cart/{cartid} | Partially update cart |
| [**commerceSetCartItem**](CartApi.md#commerceSetCartItem) | **POST** /v1/commerce/cart/{cartid}/set | Set item in cart |
| [**commerceUpdateCart**](CartApi.md#commerceUpdateCart) | **PUT** /v1/commerce/cart/{cartid} | Update cart |


<a id="commerceCreateCart"></a>
# **commerceCreateCart**
> CommerceCart commerceCreateCart(commerceCart)

Create cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val commerceCart : CommerceCart =  // CommerceCart | 
try {
    val result : CommerceCart = apiInstance.commerceCreateCart(commerceCart)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceCreateCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceCreateCart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCart** | [**CommerceCart**](CommerceCart.md)|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

<a id="commerceDeleteCart"></a>
# **commerceDeleteCart**
> commerceDeleteCart(cartid)

Delete cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
try {
    apiInstance.commerceDeleteCart(cartid)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceDeleteCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceDeleteCart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cartid** | **kotlin.String**|  | |

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

<a id="commerceDiscardCart"></a>
# **commerceDiscardCart**
> CommerceCart commerceDiscardCart(cartid)

Discard cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
try {
    val result : CommerceCart = apiInstance.commerceDiscardCart(cartid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceDiscardCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceDiscardCart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cartid** | **kotlin.String**|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

<a id="commerceGetCart"></a>
# **commerceGetCart**
> CommerceCart commerceGetCart(cartid)

Get cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
try {
    val result : CommerceCart = apiInstance.commerceGetCart(cartid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceGetCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceGetCart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cartid** | **kotlin.String**|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

<a id="commerceListCarts"></a>
# **commerceListCarts**
> CommercePaginatedCarts commerceListCarts(page, display)

List carts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
try {
    val result : CommercePaginatedCarts = apiInstance.commerceListCarts(page, display)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceListCarts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceListCarts")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**| Page number (1-indexed) | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **display** | **kotlin.Int**| Number of items per page | [optional] [default to 20] |

### Return type

[**CommercePaginatedCarts**](CommercePaginatedCarts.md)

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

<a id="commercePatchCart"></a>
# **commercePatchCart**
> CommerceCart commercePatchCart(cartid, commerceCart)

Partially update cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
val commerceCart : CommerceCart =  // CommerceCart | 
try {
    val result : CommerceCart = apiInstance.commercePatchCart(cartid, commerceCart)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commercePatchCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commercePatchCart")
    e.printStackTrace()
}
```

### Parameters
| **cartid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCart** | [**CommerceCart**](CommerceCart.md)|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

<a id="commerceSetCartItem"></a>
# **commerceSetCartItem**
> CommerceCart commerceSetCartItem(cartid, commerceSetCartItemRequest)

Set item in cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
val commerceSetCartItemRequest : CommerceSetCartItemRequest =  // CommerceSetCartItemRequest | 
try {
    val result : CommerceCart = apiInstance.commerceSetCartItem(cartid, commerceSetCartItemRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceSetCartItem")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceSetCartItem")
    e.printStackTrace()
}
```

### Parameters
| **cartid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSetCartItemRequest** | [**CommerceSetCartItemRequest**](CommerceSetCartItemRequest.md)|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

<a id="commerceUpdateCart"></a>
# **commerceUpdateCart**
> CommerceCart commerceUpdateCart(cartid, commerceCart)

Update cart

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CartApi()
val cartid : kotlin.String = cartid_example // kotlin.String | 
val commerceCart : CommerceCart =  // CommerceCart | 
try {
    val result : CommerceCart = apiInstance.commerceUpdateCart(cartid, commerceCart)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CartApi#commerceUpdateCart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CartApi#commerceUpdateCart")
    e.printStackTrace()
}
```

### Parameters
| **cartid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceCart** | [**CommerceCart**](CommerceCart.md)|  | |

### Return type

[**CommerceCart**](CommerceCart.md)

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

