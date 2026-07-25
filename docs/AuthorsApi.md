# AuthorsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authorsConnectAuthor**](AuthorsApi.md#authorsConnectAuthor) | **POST** /v1/authors/connect | Connect GitHub |
| [**authorsGetMyAuthors**](AuthorsApi.md#authorsGetMyAuthors) | **GET** /v1/authors | Get my author program |
| [**authorsVerifyRepo**](AuthorsApi.md#authorsVerifyRepo) | **POST** /v1/authors/repos/verify | Verify a repo |


<a id="authorsConnectAuthor"></a>
# **authorsConnectAuthor**
> AuthorsConnectResponse authorsConnectAuthor(authorsConnectRequest)

Connect GitHub

Enrolls the caller&#39;s org as an author at status &#x60;connected&#x60;, idempotently. Links a GitHub login — from IAM&#39;s linked account (identity verified) when present, else the supplied &#x60;githubLogin&#x60; — and mints a stable verify code. Returns 201 when newly created, 200 when already connected. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthorsApi()
val authorsConnectRequest : AuthorsConnectRequest =  // AuthorsConnectRequest | 
try {
    val result : AuthorsConnectResponse = apiInstance.authorsConnectAuthor(authorsConnectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthorsApi#authorsConnectAuthor")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthorsApi#authorsConnectAuthor")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorsConnectRequest** | [**AuthorsConnectRequest**](AuthorsConnectRequest.md)|  | [optional] |

### Return type

[**AuthorsConnectResponse**](AuthorsConnectResponse.md)

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

<a id="authorsGetMyAuthors"></a>
# **authorsGetMyAuthors**
> AuthorsGetMyAuthors200Response authorsGetMyAuthors()

Get my author program

Returns the caller org&#39;s author dashboard. If the org has not connected, a \&quot;not enrolled\&quot; shape is returned (&#x60;isAuthor: false&#x60;) so the console shows the connect form. For an APPROVED author, an opportunistic accrual sweep runs first so the dashboard is self-updating. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthorsApi()
try {
    val result : AuthorsGetMyAuthors200Response = apiInstance.authorsGetMyAuthors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthorsApi#authorsGetMyAuthors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthorsApi#authorsGetMyAuthors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AuthorsGetMyAuthors200Response**](AuthorsGetMyAuthors200Response.md)

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

<a id="authorsVerifyRepo"></a>
# **authorsVerifyRepo**
> AuthorsVerifyRepoResponse authorsVerifyRepo(authorsVerifyRepoRequest)

Verify a repo

Verifies the caller owns a repo and records it as a verified author repo. Ownership is proven by an IAM-linked GitHub token (admin/push) OR a &#x60;hanzo.json&#x60; on the default branch carrying the author&#39;s verify code. The author must have connected first. Returns 201 when newly verified, 200 when already recorded. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AuthorsApi()
val authorsVerifyRepoRequest : AuthorsVerifyRepoRequest =  // AuthorsVerifyRepoRequest | 
try {
    val result : AuthorsVerifyRepoResponse = apiInstance.authorsVerifyRepo(authorsVerifyRepoRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthorsApi#authorsVerifyRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthorsApi#authorsVerifyRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorsVerifyRepoRequest** | [**AuthorsVerifyRepoRequest**](AuthorsVerifyRepoRequest.md)|  | |

### Return type

[**AuthorsVerifyRepoResponse**](AuthorsVerifyRepoResponse.md)

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

