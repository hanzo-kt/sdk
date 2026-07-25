# StoreApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateStore**](StoreApi.md#commerceCreateStore) | **POST** /v1/commerce/store | Create store |
| [**commerceCreateStoreListing**](StoreApi.md#commerceCreateStoreListing) | **POST** /v1/commerce/store/{storeid}/listing/{key} | Create store listing |
| [**commerceDeleteStoreListing**](StoreApi.md#commerceDeleteStoreListing) | **DELETE** /v1/commerce/store/{storeid}/listing/{key} | Delete store listing |
| [**commerceGetStore**](StoreApi.md#commerceGetStore) | **GET** /v1/commerce/store/{storeid} | Get store |
| [**commerceGetStoreListing**](StoreApi.md#commerceGetStoreListing) | **GET** /v1/commerce/store/{storeid}/listing/{key} | Get store listing |
| [**commerceGetStoreProduct**](StoreApi.md#commerceGetStoreProduct) | **GET** /v1/commerce/store/{storeid}/product/{key} | Get store product |
| [**commerceGetStoreVariant**](StoreApi.md#commerceGetStoreVariant) | **GET** /v1/commerce/store/{storeid}/variant/{key} | Get store variant |
| [**commerceListStoreListings**](StoreApi.md#commerceListStoreListings) | **GET** /v1/commerce/store/{storeid}/listing | List store listings |
| [**commerceListStores**](StoreApi.md#commerceListStores) | **GET** /v1/commerce/store | List stores |
| [**commercePatchStoreListing**](StoreApi.md#commercePatchStoreListing) | **PATCH** /v1/commerce/store/{storeid}/listing/{key} | Partially update store listing |
| [**commerceStoreAuthorize**](StoreApi.md#commerceStoreAuthorize) | **POST** /v1/commerce/store/{storeid}/checkout/authorize | Authorize payment via store |
| [**commerceStoreCharge**](StoreApi.md#commerceStoreCharge) | **POST** /v1/commerce/store/{storeid}/checkout/charge | Charge payment via store |
| [**commerceUpdateStoreListing**](StoreApi.md#commerceUpdateStoreListing) | **PUT** /v1/commerce/store/{storeid}/listing/{key} | Update store listing |


<a id="commerceCreateStore"></a>
# **commerceCreateStore**
> CommerceStore commerceCreateStore(commerceStore)

Create store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val commerceStore : CommerceStore =  // CommerceStore | 
try {
    val result : CommerceStore = apiInstance.commerceCreateStore(commerceStore)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceCreateStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceCreateStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceStore** | [**CommerceStore**](CommerceStore.md)|  | |

### Return type

[**CommerceStore**](CommerceStore.md)

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

<a id="commerceCreateStoreListing"></a>
# **commerceCreateStoreListing**
> CommerceListing commerceCreateStoreListing(storeid, key, commerceListing)

Create store listing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val commerceListing : CommerceListing =  // CommerceListing | 
try {
    val result : CommerceListing = apiInstance.commerceCreateStoreListing(storeid, key, commerceListing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceCreateStoreListing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceCreateStoreListing")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceListing** | [**CommerceListing**](CommerceListing.md)|  | |

### Return type

[**CommerceListing**](CommerceListing.md)

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

<a id="commerceDeleteStoreListing"></a>
# **commerceDeleteStoreListing**
> commerceDeleteStoreListing(storeid, key)

Delete store listing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    apiInstance.commerceDeleteStoreListing(storeid, key)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceDeleteStoreListing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceDeleteStoreListing")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="commerceGetStore"></a>
# **commerceGetStore**
> CommerceStore commerceGetStore(storeid)

Get store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
try {
    val result : CommerceStore = apiInstance.commerceGetStore(storeid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceGetStore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceGetStore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **storeid** | **kotlin.String**|  | |

### Return type

[**CommerceStore**](CommerceStore.md)

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

<a id="commerceGetStoreListing"></a>
# **commerceGetStoreListing**
> CommerceListing commerceGetStoreListing(storeid, key)

Get store listing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : CommerceListing = apiInstance.commerceGetStoreListing(storeid, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceGetStoreListing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceGetStoreListing")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

### Return type

[**CommerceListing**](CommerceListing.md)

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

<a id="commerceGetStoreProduct"></a>
# **commerceGetStoreProduct**
> CommerceProduct commerceGetStoreProduct(storeid, key)

Get store product

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : CommerceProduct = apiInstance.commerceGetStoreProduct(storeid, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceGetStoreProduct")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceGetStoreProduct")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="commerceGetStoreVariant"></a>
# **commerceGetStoreVariant**
> CommerceVariant commerceGetStoreVariant(storeid, key)

Get store variant

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : CommerceVariant = apiInstance.commerceGetStoreVariant(storeid, key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceGetStoreVariant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceGetStoreVariant")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

### Return type

[**CommerceVariant**](CommerceVariant.md)

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

<a id="commerceListStoreListings"></a>
# **commerceListStoreListings**
> kotlin.collections.List&lt;CommerceListing&gt; commerceListStoreListings(storeid)

List store listings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceListing> = apiInstance.commerceListStoreListings(storeid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceListStoreListings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceListStoreListings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **storeid** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceListing&gt;**](CommerceListing.md)

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

<a id="commerceListStores"></a>
# **commerceListStores**
> CommercePaginatedStores commerceListStores(page, display)

List stores

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val page : kotlin.Int = 56 // kotlin.Int | Page number (1-indexed)
val display : kotlin.Int = 56 // kotlin.Int | Number of items per page
try {
    val result : CommercePaginatedStores = apiInstance.commerceListStores(page, display)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceListStores")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceListStores")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**| Page number (1-indexed) | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **display** | **kotlin.Int**| Number of items per page | [optional] [default to 20] |

### Return type

[**CommercePaginatedStores**](CommercePaginatedStores.md)

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

<a id="commercePatchStoreListing"></a>
# **commercePatchStoreListing**
> CommerceListing commercePatchStoreListing(storeid, key, commerceListing)

Partially update store listing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val commerceListing : CommerceListing =  // CommerceListing | 
try {
    val result : CommerceListing = apiInstance.commercePatchStoreListing(storeid, key, commerceListing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commercePatchStoreListing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commercePatchStoreListing")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceListing** | [**CommerceListing**](CommerceListing.md)|  | |

### Return type

[**CommerceListing**](CommerceListing.md)

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

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceStoreAuthorize(storeid, commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceStoreAuthorize")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceStoreAuthorize")
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

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val commerceCheckoutRequest : CommerceCheckoutRequest =  // CommerceCheckoutRequest | 
try {
    val result : CommerceOrder = apiInstance.commerceStoreCharge(storeid, commerceCheckoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceStoreCharge")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceStoreCharge")
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

<a id="commerceUpdateStoreListing"></a>
# **commerceUpdateStoreListing**
> CommerceListing commerceUpdateStoreListing(storeid, key, commerceListing)

Update store listing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreApi()
val storeid : kotlin.String = storeid_example // kotlin.String | 
val key : kotlin.String = key_example // kotlin.String | 
val commerceListing : CommerceListing =  // CommerceListing | 
try {
    val result : CommerceListing = apiInstance.commerceUpdateStoreListing(storeid, key, commerceListing)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreApi#commerceUpdateStoreListing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreApi#commerceUpdateStoreListing")
    e.printStackTrace()
}
```

### Parameters
| **storeid** | **kotlin.String**|  | |
| **key** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceListing** | [**CommerceListing**](CommerceListing.md)|  | |

### Return type

[**CommerceListing**](CommerceListing.md)

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

