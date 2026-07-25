# TeamsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsAddTeamUser**](TeamsApi.md#analyticsAddTeamUser) | **POST** /v1/analytics/teams/{teamId}/users | Add a user to a team |
| [**analyticsCreateTeam**](TeamsApi.md#analyticsCreateTeam) | **POST** /v1/analytics/teams | Create a new team |
| [**analyticsDeleteTeam**](TeamsApi.md#analyticsDeleteTeam) | **DELETE** /v1/analytics/teams/{teamId} | Delete team (owner only) |
| [**analyticsGetTeam**](TeamsApi.md#analyticsGetTeam) | **GET** /v1/analytics/teams/{teamId} | Get team by ID (includes members) |
| [**analyticsGetTeamUser**](TeamsApi.md#analyticsGetTeamUser) | **GET** /v1/analytics/teams/{teamId}/users/{userId} | Get a team member |
| [**analyticsGetTeamUsers**](TeamsApi.md#analyticsGetTeamUsers) | **GET** /v1/analytics/teams/{teamId}/users | List team members |
| [**analyticsGetTeamWebsites**](TeamsApi.md#analyticsGetTeamWebsites) | **GET** /v1/analytics/teams/{teamId}/websites | List websites belonging to a team |
| [**analyticsJoinTeam**](TeamsApi.md#analyticsJoinTeam) | **POST** /v1/analytics/teams/join | Join a team using an access code |
| [**analyticsRemoveTeamUser**](TeamsApi.md#analyticsRemoveTeamUser) | **DELETE** /v1/analytics/teams/{teamId}/users/{userId} | Remove user from team |
| [**analyticsUpdateTeam**](TeamsApi.md#analyticsUpdateTeam) | **POST** /v1/analytics/teams/{teamId} | Update team (owner only) |
| [**analyticsUpdateTeamUser**](TeamsApi.md#analyticsUpdateTeamUser) | **POST** /v1/analytics/teams/{teamId}/users/{userId} | Update team member role (owner only) |
| [**gatewayCreateTeam**](TeamsApi.md#gatewayCreateTeam) | **POST** /v1/gateway/team/new | Create team |
| [**gatewayGetTeamInfo**](TeamsApi.md#gatewayGetTeamInfo) | **GET** /v1/gateway/team/info | Get team info |
| [**gatewayListTeams**](TeamsApi.md#gatewayListTeams) | **GET** /v1/gateway/team/list | List teams |


<a id="analyticsAddTeamUser"></a>
# **analyticsAddTeamUser**
> AnalyticsTeamUser analyticsAddTeamUser(teamId, analyticsAddTeamUserRequest)

Add a user to a team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsAddTeamUserRequest : AnalyticsAddTeamUserRequest =  // AnalyticsAddTeamUserRequest | 
try {
    val result : AnalyticsTeamUser = apiInstance.analyticsAddTeamUser(teamId, analyticsAddTeamUserRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsAddTeamUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsAddTeamUser")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsAddTeamUserRequest** | [**AnalyticsAddTeamUserRequest**](AnalyticsAddTeamUserRequest.md)|  | |

### Return type

[**AnalyticsTeamUser**](AnalyticsTeamUser.md)

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

<a id="analyticsCreateTeam"></a>
# **analyticsCreateTeam**
> AnalyticsTeam analyticsCreateTeam(analyticsCreateTeamRequest)

Create a new team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val analyticsCreateTeamRequest : AnalyticsCreateTeamRequest =  // AnalyticsCreateTeamRequest | 
try {
    val result : AnalyticsTeam = apiInstance.analyticsCreateTeam(analyticsCreateTeamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsCreateTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsCreateTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsCreateTeamRequest** | [**AnalyticsCreateTeamRequest**](AnalyticsCreateTeamRequest.md)|  | |

### Return type

[**AnalyticsTeam**](AnalyticsTeam.md)

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

<a id="analyticsDeleteTeam"></a>
# **analyticsDeleteTeam**
> kotlin.Any analyticsDeleteTeam(teamId)

Delete team (owner only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsDeleteTeam(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsDeleteTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsDeleteTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **java.util.UUID**|  | |

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

<a id="analyticsGetTeam"></a>
# **analyticsGetTeam**
> AnalyticsTeam analyticsGetTeam(teamId)

Get team by ID (includes members)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsTeam = apiInstance.analyticsGetTeam(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsGetTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsGetTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsTeam**](AnalyticsTeam.md)

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

<a id="analyticsGetTeamUser"></a>
# **analyticsGetTeamUser**
> AnalyticsTeamUser analyticsGetTeamUser(teamId, userId)

Get a team member

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsTeamUser = apiInstance.analyticsGetTeamUser(teamId, userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsGetTeamUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsGetTeamUser")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsTeamUser**](AnalyticsTeamUser.md)

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

<a id="analyticsGetTeamUsers"></a>
# **analyticsGetTeamUsers**
> kotlin.collections.List&lt;AnalyticsTeamUser&gt; analyticsGetTeamUsers(teamId, page, pageSize, orderBy, search)

List team members

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsTeamUser> = apiInstance.analyticsGetTeamUsers(teamId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsGetTeamUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsGetTeamUsers")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsTeamUser&gt;**](AnalyticsTeamUser.md)

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

<a id="analyticsGetTeamWebsites"></a>
# **analyticsGetTeamWebsites**
> kotlin.collections.List&lt;AnalyticsWebsite&gt; analyticsGetTeamWebsites(teamId, page, pageSize, orderBy, search)

List websites belonging to a team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsWebsite> = apiInstance.analyticsGetTeamWebsites(teamId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsGetTeamWebsites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsGetTeamWebsites")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
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

<a id="analyticsJoinTeam"></a>
# **analyticsJoinTeam**
> AnalyticsTeamUser analyticsJoinTeam(analyticsJoinTeamRequest)

Join a team using an access code

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val analyticsJoinTeamRequest : AnalyticsJoinTeamRequest =  // AnalyticsJoinTeamRequest | 
try {
    val result : AnalyticsTeamUser = apiInstance.analyticsJoinTeam(analyticsJoinTeamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsJoinTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsJoinTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsJoinTeamRequest** | [**AnalyticsJoinTeamRequest**](AnalyticsJoinTeamRequest.md)|  | |

### Return type

[**AnalyticsTeamUser**](AnalyticsTeamUser.md)

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

<a id="analyticsRemoveTeamUser"></a>
# **analyticsRemoveTeamUser**
> kotlin.Any analyticsRemoveTeamUser(teamId, userId)

Remove user from team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsRemoveTeamUser(teamId, userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsRemoveTeamUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsRemoveTeamUser")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

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

<a id="analyticsUpdateTeam"></a>
# **analyticsUpdateTeam**
> AnalyticsTeam analyticsUpdateTeam(teamId, analyticsUpdateTeamRequest)

Update team (owner only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsUpdateTeamRequest : AnalyticsUpdateTeamRequest =  // AnalyticsUpdateTeamRequest | 
try {
    val result : AnalyticsTeam = apiInstance.analyticsUpdateTeam(teamId, analyticsUpdateTeamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsUpdateTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsUpdateTeam")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsUpdateTeamRequest** | [**AnalyticsUpdateTeamRequest**](AnalyticsUpdateTeamRequest.md)|  | |

### Return type

[**AnalyticsTeam**](AnalyticsTeam.md)

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

<a id="analyticsUpdateTeamUser"></a>
# **analyticsUpdateTeamUser**
> AnalyticsTeamUser analyticsUpdateTeamUser(teamId, userId, analyticsUpdateTeamUserRequest)

Update team member role (owner only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsUpdateTeamUserRequest : AnalyticsUpdateTeamUserRequest =  // AnalyticsUpdateTeamUserRequest | 
try {
    val result : AnalyticsTeamUser = apiInstance.analyticsUpdateTeamUser(teamId, userId, analyticsUpdateTeamUserRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#analyticsUpdateTeamUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#analyticsUpdateTeamUser")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **java.util.UUID**|  | |
| **userId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsUpdateTeamUserRequest** | [**AnalyticsUpdateTeamUserRequest**](AnalyticsUpdateTeamUserRequest.md)|  | |

### Return type

[**AnalyticsTeamUser**](AnalyticsTeamUser.md)

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

<a id="gatewayCreateTeam"></a>
# **gatewayCreateTeam**
> GatewayTeam gatewayCreateTeam(gatewayCreateTeamRequest)

Create team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val gatewayCreateTeamRequest : GatewayCreateTeamRequest =  // GatewayCreateTeamRequest | 
try {
    val result : GatewayTeam = apiInstance.gatewayCreateTeam(gatewayCreateTeamRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#gatewayCreateTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#gatewayCreateTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayCreateTeamRequest** | [**GatewayCreateTeamRequest**](GatewayCreateTeamRequest.md)|  | |

### Return type

[**GatewayTeam**](GatewayTeam.md)

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

<a id="gatewayGetTeamInfo"></a>
# **gatewayGetTeamInfo**
> GatewayTeam gatewayGetTeamInfo(teamId)

Get team info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    val result : GatewayTeam = apiInstance.gatewayGetTeamInfo(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#gatewayGetTeamInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#gatewayGetTeamInfo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

[**GatewayTeam**](GatewayTeam.md)

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

<a id="gatewayListTeams"></a>
# **gatewayListTeams**
> kotlin.collections.List&lt;GatewayTeam&gt; gatewayListTeams()

List teams

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TeamsApi()
try {
    val result : kotlin.collections.List<GatewayTeam> = apiInstance.gatewayListTeams()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#gatewayListTeams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#gatewayListTeams")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;GatewayTeam&gt;**](GatewayTeam.md)

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

