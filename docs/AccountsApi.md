# AccountsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqGetAccount**](AccountsApi.md#mqGetAccount) | **GET** /v1/mq/accounts/{id} | Get account info |
| [**mqListAccountConnections**](AccountsApi.md#mqListAccountConnections) | **GET** /v1/mq/accounts/{id}/connections | List account connections |
| [**mqListAccounts**](AccountsApi.md#mqListAccounts) | **GET** /v1/mq/accounts | List accounts |


<a id="mqGetAccount"></a>
# **mqGetAccount**
> MqAccount mqGetAccount(id)

Get account info

Returns account details including connection count, subscription count, data throughput, and slow consumer metrics. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountsApi()
val id : kotlin.String = id_example // kotlin.String | Account ID (maps to IAM org_id).
try {
    val result : MqAccount = apiInstance.mqGetAccount(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#mqGetAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#mqGetAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Account ID (maps to IAM org_id). | |

### Return type

[**MqAccount**](MqAccount.md)

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

<a id="mqListAccountConnections"></a>
# **mqListAccountConnections**
> MqListAccountConnections200Response mqListAccountConnections(id, limit, offset)

List account connections

Returns all active connections for the account.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountsApi()
val id : kotlin.String = id_example // kotlin.String | Account ID (maps to IAM org_id).
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListAccountConnections200Response = apiInstance.mqListAccountConnections(id, limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#mqListAccountConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#mqListAccountConnections")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Account ID (maps to IAM org_id). | |
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListAccountConnections200Response**](MqListAccountConnections200Response.md)

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

<a id="mqListAccounts"></a>
# **mqListAccounts**
> MqListAccounts200Response mqListAccounts(limit, offset)

List accounts

Returns all MQ accounts visible to the authenticated user. Each account maps to a Hanzo IAM organization. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AccountsApi()
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
try {
    val result : MqListAccounts200Response = apiInstance.mqListAccounts(limit, offset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AccountsApi#mqListAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AccountsApi#mqListAccounts")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |

### Return type

[**MqListAccounts200Response**](MqListAccounts200Response.md)

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

