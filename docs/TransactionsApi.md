# TransactionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateHold**](TransactionsApi.md#commerceCreateHold) | **POST** /v1/commerce/transaction/hold | Create hold |
| [**commerceCreateTransaction**](TransactionsApi.md#commerceCreateTransaction) | **POST** /v1/commerce/transaction | Create transaction |
| [**commerceListTransactions**](TransactionsApi.md#commerceListTransactions) | **GET** /v1/commerce/transaction/{kind}/{id} | List transactions for entity |
| [**commerceRemoveHold**](TransactionsApi.md#commerceRemoveHold) | **DELETE** /v1/commerce/transaction/hold/{id} | Remove hold |


<a id="commerceCreateHold"></a>
# **commerceCreateHold**
> CommerceTransaction commerceCreateHold(commerceTransaction)

Create hold

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TransactionsApi()
val commerceTransaction : CommerceTransaction =  // CommerceTransaction | 
try {
    val result : CommerceTransaction = apiInstance.commerceCreateHold(commerceTransaction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TransactionsApi#commerceCreateHold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransactionsApi#commerceCreateHold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceTransaction** | [**CommerceTransaction**](CommerceTransaction.md)|  | |

### Return type

[**CommerceTransaction**](CommerceTransaction.md)

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

<a id="commerceCreateTransaction"></a>
# **commerceCreateTransaction**
> CommerceTransaction commerceCreateTransaction(commerceTransaction)

Create transaction

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TransactionsApi()
val commerceTransaction : CommerceTransaction =  // CommerceTransaction | 
try {
    val result : CommerceTransaction = apiInstance.commerceCreateTransaction(commerceTransaction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TransactionsApi#commerceCreateTransaction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransactionsApi#commerceCreateTransaction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceTransaction** | [**CommerceTransaction**](CommerceTransaction.md)|  | |

### Return type

[**CommerceTransaction**](CommerceTransaction.md)

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

<a id="commerceListTransactions"></a>
# **commerceListTransactions**
> kotlin.collections.List&lt;CommerceTransaction&gt; commerceListTransactions(kind, id)

List transactions for entity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TransactionsApi()
val kind : kotlin.String = kind_example // kotlin.String | 
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.collections.List<CommerceTransaction> = apiInstance.commerceListTransactions(kind, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TransactionsApi#commerceListTransactions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransactionsApi#commerceListTransactions")
    e.printStackTrace()
}
```

### Parameters
| **kind** | **kotlin.String**|  | [enum: user, order, wallet] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;CommerceTransaction&gt;**](CommerceTransaction.md)

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

<a id="commerceRemoveHold"></a>
# **commerceRemoveHold**
> commerceRemoveHold(id)

Remove hold

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TransactionsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.commerceRemoveHold(id)
} catch (e: ClientException) {
    println("4xx response calling TransactionsApi#commerceRemoveHold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TransactionsApi#commerceRemoveHold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

