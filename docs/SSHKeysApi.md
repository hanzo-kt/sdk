# SSHKeysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gitDeleteGitKey**](SSHKeysApi.md#gitDeleteGitKey) | **DELETE** /v1/git/keys/{id} | Remove an SSH key |
| [**gitListGitKeys**](SSHKeysApi.md#gitListGitKeys) | **GET** /v1/git/keys | List the tenant&#39;s SSH keys |
| [**gitRegisterGitKey**](SSHKeysApi.md#gitRegisterGitKey) | **POST** /v1/git/keys | Register an SSH public key |


<a id="gitDeleteGitKey"></a>
# **gitDeleteGitKey**
> gitDeleteGitKey(id)

Remove an SSH key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SSHKeysApi()
val id : kotlin.String = id_example // kotlin.String | Key id
try {
    apiInstance.gitDeleteGitKey(id)
} catch (e: ClientException) {
    println("4xx response calling SSHKeysApi#gitDeleteGitKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SSHKeysApi#gitDeleteGitKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Key id | |

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

<a id="gitListGitKeys"></a>
# **gitListGitKeys**
> GitListGitKeys200Response gitListGitKeys()

List the tenant&#39;s SSH keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SSHKeysApi()
try {
    val result : GitListGitKeys200Response = apiInstance.gitListGitKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SSHKeysApi#gitListGitKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SSHKeysApi#gitListGitKeys")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GitListGitKeys200Response**](GitListGitKeys200Response.md)

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

<a id="gitRegisterGitKey"></a>
# **gitRegisterGitKey**
> GitKey gitRegisterGitKey(gitRegisterKey)

Register an SSH public key

Registers an OpenSSH public key for the tenant. The key is validated, canonicalized, and stored with its SHA256 fingerprint (the global unique handle). A key belongs to exactly one org; re-registering it under another org is a 409. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SSHKeysApi()
val gitRegisterKey : GitRegisterKey =  // GitRegisterKey | 
try {
    val result : GitKey = apiInstance.gitRegisterGitKey(gitRegisterKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SSHKeysApi#gitRegisterGitKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SSHKeysApi#gitRegisterGitKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gitRegisterKey** | [**GitRegisterKey**](GitRegisterKey.md)|  | |

### Return type

[**GitKey**](GitKey.md)

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

