# DirectoriesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**didCreateTeam**](DirectoriesApi.md#didCreateTeam) | **POST** /v1/did/directories/{organization}/teams | Create a team |
| [**didGetDirectory**](DirectoriesApi.md#didGetDirectory) | **GET** /v1/did/directories/{organization} | Get organization directory |
| [**didGetTeamMembers**](DirectoriesApi.md#didGetTeamMembers) | **GET** /v1/did/directories/{organization}/teams/{team} | Get team members |
| [**didListTeams**](DirectoriesApi.md#didListTeams) | **GET** /v1/did/directories/{organization}/teams | List teams |


<a id="didCreateTeam"></a>
# **didCreateTeam**
> DidTeam didCreateTeam(organization, didCreateTeamRequest)

Create a team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DirectoriesApi()
val organization : kotlin.String = organization_example // kotlin.String | 
val didCreateTeamRequest : DidCreateTeamRequest =  // DidCreateTeamRequest | 
try {
    val result : DidTeam = apiInstance.didCreateTeam(organization, didCreateTeamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DirectoriesApi#didCreateTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DirectoriesApi#didCreateTeam")
    e.printStackTrace()
}
```

### Parameters
| **organization** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **didCreateTeamRequest** | [**DidCreateTeamRequest**](DidCreateTeamRequest.md)|  | |

### Return type

[**DidTeam**](DidTeam.md)

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

<a id="didGetDirectory"></a>
# **didGetDirectory**
> DidDirectory didGetDirectory(organization)

Get organization directory

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DirectoriesApi()
val organization : kotlin.String = organization_example // kotlin.String | 
try {
    val result : DidDirectory = apiInstance.didGetDirectory(organization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DirectoriesApi#didGetDirectory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DirectoriesApi#didGetDirectory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization** | **kotlin.String**|  | |

### Return type

[**DidDirectory**](DidDirectory.md)

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

<a id="didGetTeamMembers"></a>
# **didGetTeamMembers**
> DidGetTeamMembers200Response didGetTeamMembers(organization, team)

Get team members

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DirectoriesApi()
val organization : kotlin.String = organization_example // kotlin.String | 
val team : kotlin.String = team_example // kotlin.String | 
try {
    val result : DidGetTeamMembers200Response = apiInstance.didGetTeamMembers(organization, team)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DirectoriesApi#didGetTeamMembers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DirectoriesApi#didGetTeamMembers")
    e.printStackTrace()
}
```

### Parameters
| **organization** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team** | **kotlin.String**|  | |

### Return type

[**DidGetTeamMembers200Response**](DidGetTeamMembers200Response.md)

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

<a id="didListTeams"></a>
# **didListTeams**
> DidListTeams200Response didListTeams(organization)

List teams

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DirectoriesApi()
val organization : kotlin.String = organization_example // kotlin.String | 
try {
    val result : DidListTeams200Response = apiInstance.didListTeams(organization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DirectoriesApi#didListTeams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DirectoriesApi#didListTeams")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization** | **kotlin.String**|  | |

### Return type

[**DidListTeams200Response**](DidListTeams200Response.md)

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

