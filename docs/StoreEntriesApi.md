# StoreEntriesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoDeleteStoreEntry**](StoreEntriesApi.md#autoDeleteStoreEntry) | **DELETE** /v1/auto/store-entries/{key} | Delete a store entry |
| [**autoGetStoreEntry**](StoreEntriesApi.md#autoGetStoreEntry) | **GET** /v1/auto/store-entries/{key} | Get a store entry by key |
| [**autoListStoreEntries**](StoreEntriesApi.md#autoListStoreEntries) | **GET** /v1/auto/store-entries | List store entries |
| [**autoUpsertStoreEntry**](StoreEntriesApi.md#autoUpsertStoreEntry) | **POST** /v1/auto/store-entries | Create or update a store entry |
| [**flowDeleteStoreEntry**](StoreEntriesApi.md#flowDeleteStoreEntry) | **DELETE** /v1/flow/store-entries/{key} | Delete a store entry |
| [**flowGetStoreEntry**](StoreEntriesApi.md#flowGetStoreEntry) | **GET** /v1/flow/store-entries/{key} | Get a store entry by key |
| [**flowListStoreEntries**](StoreEntriesApi.md#flowListStoreEntries) | **GET** /v1/flow/store-entries | List store entries |
| [**flowUpsertStoreEntry**](StoreEntriesApi.md#flowUpsertStoreEntry) | **POST** /v1/flow/store-entries | Create or update a store entry |


<a id="autoDeleteStoreEntry"></a>
# **autoDeleteStoreEntry**
> autoDeleteStoreEntry(key)

Delete a store entry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    apiInstance.autoDeleteStoreEntry(key)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#autoDeleteStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#autoDeleteStoreEntry")
    e.printStackTrace()
}
```

### Parameters
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
 - **Accept**: Not defined

<a id="autoGetStoreEntry"></a>
# **autoGetStoreEntry**
> kotlin.Any autoGetStoreEntry(key)

Get a store entry by key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetStoreEntry(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#autoGetStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#autoGetStoreEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="autoListStoreEntries"></a>
# **autoListStoreEntries**
> kotlin.Any autoListStoreEntries()

List store entries

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
try {
    val result : kotlin.Any = apiInstance.autoListStoreEntries()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#autoListStoreEntries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#autoListStoreEntries")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="autoUpsertStoreEntry"></a>
# **autoUpsertStoreEntry**
> kotlin.Any autoUpsertStoreEntry(autoUpsertStoreEntryRequest)

Create or update a store entry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val autoUpsertStoreEntryRequest : AutoUpsertStoreEntryRequest =  // AutoUpsertStoreEntryRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpsertStoreEntry(autoUpsertStoreEntryRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#autoUpsertStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#autoUpsertStoreEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpsertStoreEntryRequest** | [**AutoUpsertStoreEntryRequest**](AutoUpsertStoreEntryRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowDeleteStoreEntry"></a>
# **flowDeleteStoreEntry**
> flowDeleteStoreEntry(key)

Delete a store entry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    apiInstance.flowDeleteStoreEntry(key)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#flowDeleteStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#flowDeleteStoreEntry")
    e.printStackTrace()
}
```

### Parameters
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
 - **Accept**: Not defined

<a id="flowGetStoreEntry"></a>
# **flowGetStoreEntry**
> kotlin.Any flowGetStoreEntry(key)

Get a store entry by key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetStoreEntry(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#flowGetStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#flowGetStoreEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

<a id="flowListStoreEntries"></a>
# **flowListStoreEntries**
> kotlin.Any flowListStoreEntries(cursor, limit)

List store entries

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.flowListStoreEntries(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#flowListStoreEntries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#flowListStoreEntries")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

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

<a id="flowUpsertStoreEntry"></a>
# **flowUpsertStoreEntry**
> FlowStoreEntry flowUpsertStoreEntry(autoUpsertStoreEntryRequest)

Create or update a store entry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StoreEntriesApi()
val autoUpsertStoreEntryRequest : AutoUpsertStoreEntryRequest =  // AutoUpsertStoreEntryRequest | 
try {
    val result : FlowStoreEntry = apiInstance.flowUpsertStoreEntry(autoUpsertStoreEntryRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StoreEntriesApi#flowUpsertStoreEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StoreEntriesApi#flowUpsertStoreEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpsertStoreEntryRequest** | [**AutoUpsertStoreEntryRequest**](AutoUpsertStoreEntryRequest.md)|  | |

### Return type

[**FlowStoreEntry**](FlowStoreEntry.md)

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

