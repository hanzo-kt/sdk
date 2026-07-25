# MeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsChangeMyPassword**](MeApi.md#analyticsChangeMyPassword) | **POST** /v1/analytics/me/password | Change current user password |
| [**analyticsGetMe**](MeApi.md#analyticsGetMe) | **GET** /v1/analytics/me | Get current authenticated user info |
| [**analyticsGetMyTeams**](MeApi.md#analyticsGetMyTeams) | **GET** /v1/analytics/me/teams | List teams for the current user |
| [**analyticsGetMyWebsites**](MeApi.md#analyticsGetMyWebsites) | **GET** /v1/analytics/me/websites | List websites for the current user |


<a id="analyticsChangeMyPassword"></a>
# **analyticsChangeMyPassword**
> AnalyticsUser analyticsChangeMyPassword(analyticsChangeMyPasswordRequest)

Change current user password

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MeApi()
val analyticsChangeMyPasswordRequest : AnalyticsChangeMyPasswordRequest =  // AnalyticsChangeMyPasswordRequest | 
try {
    val result : AnalyticsUser = apiInstance.analyticsChangeMyPassword(analyticsChangeMyPasswordRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MeApi#analyticsChangeMyPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MeApi#analyticsChangeMyPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsChangeMyPasswordRequest** | [**AnalyticsChangeMyPasswordRequest**](AnalyticsChangeMyPasswordRequest.md)|  | |

### Return type

[**AnalyticsUser**](AnalyticsUser.md)

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

<a id="analyticsGetMe"></a>
# **analyticsGetMe**
> AnalyticsGetMe200Response analyticsGetMe()

Get current authenticated user info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MeApi()
try {
    val result : AnalyticsGetMe200Response = apiInstance.analyticsGetMe()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MeApi#analyticsGetMe")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MeApi#analyticsGetMe")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AnalyticsGetMe200Response**](AnalyticsGetMe200Response.md)

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

<a id="analyticsGetMyTeams"></a>
# **analyticsGetMyTeams**
> kotlin.collections.List&lt;AnalyticsTeam&gt; analyticsGetMyTeams(page, pageSize, orderBy, search)

List teams for the current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MeApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsTeam> = apiInstance.analyticsGetMyTeams(page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MeApi#analyticsGetMyTeams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MeApi#analyticsGetMyTeams")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsTeam&gt;**](AnalyticsTeam.md)

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

<a id="analyticsGetMyWebsites"></a>
# **analyticsGetMyWebsites**
> kotlin.collections.List&lt;AnalyticsWebsite&gt; analyticsGetMyWebsites(page, pageSize, orderBy, search)

List websites for the current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MeApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsWebsite> = apiInstance.analyticsGetMyWebsites(page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MeApi#analyticsGetMyWebsites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MeApi#analyticsGetMyWebsites")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsWebsite&gt;**](AnalyticsWebsite.md)

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

