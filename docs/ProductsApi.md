# ProductsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateProduct**](ProductsApi.md#commerceCreateProduct) | **POST** /v1/commerce/product | Create product |
| [**commerceDeleteProduct**](ProductsApi.md#commerceDeleteProduct) | **DELETE** /v1/commerce/product/{productid} | Delete product |
| [**commerceGetProduct**](ProductsApi.md#commerceGetProduct) | **GET** /v1/commerce/product/{productid} | Get product |
| [**commerceListProducts**](ProductsApi.md#commerceListProducts) | **GET** /v1/commerce/product | List products |
| [**commercePatchProduct**](ProductsApi.md#commercePatchProduct) | **PATCH** /v1/commerce/product/{productid} | Partially update product |
| [**commerceUpdateProduct**](ProductsApi.md#commerceUpdateProduct) | **PUT** /v1/commerce/product/{productid} | Update product |


<a id="commerceCreateProduct"></a>
# **commerceCreateProduct**
> CommerceProduct commerceCreateProduct(commerceProduct)

Create product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val commerceProduct : CommerceProduct =  // CommerceProduct | 
try {
    val result : CommerceProduct = apiInstance.commerceCreateProduct(commerceProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commerceCreateProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commerceCreateProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceProduct** | [**CommerceProduct**](CommerceProduct.md)|  | |

### Return type

[**CommerceProduct**](CommerceProduct.md)

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

<a id="commerceDeleteProduct"></a>
# **commerceDeleteProduct**
> commerceDeleteProduct(productid)

Delete product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val productid : kotlin.String = productid_example // kotlin.String | 
try {
    apiInstance.commerceDeleteProduct(productid)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commerceDeleteProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commerceDeleteProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productid** | **kotlin.String**|  | |

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

<a id="commerceGetProduct"></a>
# **commerceGetProduct**
> CommerceProduct commerceGetProduct(productid)

Get product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val productid : kotlin.String = productid_example // kotlin.String | 
try {
    val result : CommerceProduct = apiInstance.commerceGetProduct(productid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commerceGetProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commerceGetProduct")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productid** | **kotlin.String**|  | |

### Return type

[**CommerceProduct**](CommerceProduct.md)

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

<a id="commerceListProducts"></a>
# **commerceListProducts**
> CommercePaginatedProducts commerceListProducts(page, display, sort, q)

List products

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
val sort : kotlin.String = sort_example // kotlin.String | Sort field (prefix with - for descending)
val q : kotlin.String = q_example // kotlin.String | Search query
try {
    val result : CommercePaginatedProducts = apiInstance.commerceListProducts(page, display, sort, q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commerceListProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commerceListProducts")
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

[**CommercePaginatedProducts**](CommercePaginatedProducts.md)

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

<a id="commercePatchProduct"></a>
# **commercePatchProduct**
> CommerceProduct commercePatchProduct(productid, commerceProduct)

Partially update product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val productid : kotlin.String = productid_example // kotlin.String | 
val commerceProduct : CommerceProduct =  // CommerceProduct | 
try {
    val result : CommerceProduct = apiInstance.commercePatchProduct(productid, commerceProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commercePatchProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commercePatchProduct")
    e.printStackTrace()
}
```

### Parameters
| **productid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceProduct** | [**CommerceProduct**](CommerceProduct.md)|  | |

### Return type

[**CommerceProduct**](CommerceProduct.md)

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

<a id="commerceUpdateProduct"></a>
# **commerceUpdateProduct**
> CommerceProduct commerceUpdateProduct(productid, commerceProduct)

Update product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProductsApi()
val productid : kotlin.String = productid_example // kotlin.String | 
val commerceProduct : CommerceProduct =  // CommerceProduct | 
try {
    val result : CommerceProduct = apiInstance.commerceUpdateProduct(productid, commerceProduct)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductsApi#commerceUpdateProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductsApi#commerceUpdateProduct")
    e.printStackTrace()
}
```

### Parameters
| **productid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceProduct** | [**CommerceProduct**](CommerceProduct.md)|  | |

### Return type

[**CommerceProduct**](CommerceProduct.md)

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

