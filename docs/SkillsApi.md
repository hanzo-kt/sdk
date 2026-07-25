# SkillsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**botCreateSkillComment**](SkillsApi.md#botCreateSkillComment) | **POST** /v1/bot/skills/{slug}/comments | Add a comment to a skill |
| [**botDeleteSkill**](SkillsApi.md#botDeleteSkill) | **DELETE** /v1/bot/skills/{slug} | Soft-delete a skill (owner or admin only) |
| [**botDeleteSkillComment**](SkillsApi.md#botDeleteSkillComment) | **DELETE** /v1/bot/skills/{slug}/comments/{commentId} | Delete a comment (author or admin only) |
| [**botGetSkill**](SkillsApi.md#botGetSkill) | **GET** /v1/bot/skills/{slug} | Get skill details by slug |
| [**botGetSkillStarStatus**](SkillsApi.md#botGetSkillStarStatus) | **GET** /v1/bot/skills/{slug}/stars/me | Check if current user has starred this skill |
| [**botGetSkillVersionFiles**](SkillsApi.md#botGetSkillVersionFiles) | **GET** /v1/bot/skills/{slug}/versions/{version}/files | Get file listing for a specific version |
| [**botListSkillComments**](SkillsApi.md#botListSkillComments) | **GET** /v1/bot/skills/{slug}/comments | List comments on a skill |
| [**botListSkillVersions**](SkillsApi.md#botListSkillVersions) | **GET** /v1/bot/skills/{slug}/versions | List versions of a skill |
| [**botListSkills**](SkillsApi.md#botListSkills) | **GET** /v1/bot/skills | List published skills (paginated) |
| [**botPublishSkillVersion**](SkillsApi.md#botPublishSkillVersion) | **POST** /v1/bot/skills/{slug}/publish | Publish a new version of a skill (creates skill if new) |
| [**botToggleSkillStar**](SkillsApi.md#botToggleSkillStar) | **POST** /v1/bot/skills/{slug}/stars | Star or unstar a skill (toggle) |
| [**botUndeleteSkill**](SkillsApi.md#botUndeleteSkill) | **POST** /v1/bot/skills/{slug}/undelete | Restore a soft-deleted skill |


<a id="botCreateSkillComment"></a>
# **botCreateSkillComment**
> BotComment botCreateSkillComment(slug, botCreateSkillCommentRequest)

Add a comment to a skill

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val botCreateSkillCommentRequest : BotCreateSkillCommentRequest =  // BotCreateSkillCommentRequest | 
try {
    val result : BotComment = apiInstance.botCreateSkillComment(slug, botCreateSkillCommentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botCreateSkillComment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botCreateSkillComment")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **botCreateSkillCommentRequest** | [**BotCreateSkillCommentRequest**](BotCreateSkillCommentRequest.md)|  | |

### Return type

[**BotComment**](BotComment.md)

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

<a id="botDeleteSkill"></a>
# **botDeleteSkill**
> AnalyticsHeartbeat200Response botDeleteSkill(slug)

Soft-delete a skill (owner or admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botDeleteSkill(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botDeleteSkill")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botDeleteSkill")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

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

<a id="botDeleteSkillComment"></a>
# **botDeleteSkillComment**
> AnalyticsHeartbeat200Response botDeleteSkillComment(slug, commentId)

Delete a comment (author or admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val commentId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botDeleteSkillComment(slug, commentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botDeleteSkillComment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botDeleteSkillComment")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commentId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

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

<a id="botGetSkill"></a>
# **botGetSkill**
> BotSkill botGetSkill(slug)

Get skill details by slug

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotSkill = apiInstance.botGetSkill(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botGetSkill")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botGetSkill")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotSkill**](BotSkill.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botGetSkillStarStatus"></a>
# **botGetSkillStarStatus**
> BotToggleSkillStar200Response botGetSkillStarStatus(slug)

Check if current user has starred this skill

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotToggleSkillStar200Response = apiInstance.botGetSkillStarStatus(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botGetSkillStarStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botGetSkillStarStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotToggleSkillStar200Response**](BotToggleSkillStar200Response.md)

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

<a id="botGetSkillVersionFiles"></a>
# **botGetSkillVersionFiles**
> BotGetSkillVersionFiles200Response botGetSkillVersionFiles(slug, version)

Get file listing for a specific version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val version : kotlin.String = version_example // kotlin.String | 
try {
    val result : BotGetSkillVersionFiles200Response = apiInstance.botGetSkillVersionFiles(slug, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botGetSkillVersionFiles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botGetSkillVersionFiles")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.String**|  | |

### Return type

[**BotGetSkillVersionFiles200Response**](BotGetSkillVersionFiles200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListSkillComments"></a>
# **botListSkillComments**
> BotListSkillComments200Response botListSkillComments(slug)

List comments on a skill

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotListSkillComments200Response = apiInstance.botListSkillComments(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botListSkillComments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botListSkillComments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotListSkillComments200Response**](BotListSkillComments200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListSkillVersions"></a>
# **botListSkillVersions**
> BotListSkillVersions200Response botListSkillVersions(slug, limit)

List versions of a skill

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BotListSkillVersions200Response = apiInstance.botListSkillVersions(slug, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botListSkillVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botListSkillVersions")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |

### Return type

[**BotListSkillVersions200Response**](BotListSkillVersions200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botListSkills"></a>
# **botListSkills**
> BotListSkills200Response botListSkills(sort, limit, cursor, batch)

List published skills (paginated)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val sort : kotlin.String = sort_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val cursor : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | Cursor for pagination (updatedAt ISO timestamp)
val batch : kotlin.String = batch_example // kotlin.String | Filter by batch grouping key
try {
    val result : BotListSkills200Response = apiInstance.botListSkills(sort, limit, cursor, batch)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botListSkills")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botListSkills")
    e.printStackTrace()
}
```

### Parameters
| **sort** | **kotlin.String**|  | [optional] [default to Sort.updated] [enum: updated, downloads, stars, created] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| **cursor** | **java.time.OffsetDateTime**| Cursor for pagination (updatedAt ISO timestamp) | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **batch** | **kotlin.String**| Filter by batch grouping key | [optional] |

### Return type

[**BotListSkills200Response**](BotListSkills200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="botPublishSkillVersion"></a>
# **botPublishSkillVersion**
> BotPublishSkillVersion200Response botPublishSkillVersion(slug, botPublishSkillVersionRequest)

Publish a new version of a skill (creates skill if new)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val botPublishSkillVersionRequest : BotPublishSkillVersionRequest =  // BotPublishSkillVersionRequest | 
try {
    val result : BotPublishSkillVersion200Response = apiInstance.botPublishSkillVersion(slug, botPublishSkillVersionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botPublishSkillVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botPublishSkillVersion")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **botPublishSkillVersionRequest** | [**BotPublishSkillVersionRequest**](BotPublishSkillVersionRequest.md)|  | |

### Return type

[**BotPublishSkillVersion200Response**](BotPublishSkillVersion200Response.md)

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

<a id="botToggleSkillStar"></a>
# **botToggleSkillStar**
> BotToggleSkillStar200Response botToggleSkillStar(slug)

Star or unstar a skill (toggle)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : BotToggleSkillStar200Response = apiInstance.botToggleSkillStar(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botToggleSkillStar")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botToggleSkillStar")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**BotToggleSkillStar200Response**](BotToggleSkillStar200Response.md)

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

<a id="botUndeleteSkill"></a>
# **botUndeleteSkill**
> AnalyticsHeartbeat200Response botUndeleteSkill(slug)

Restore a soft-deleted skill

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SkillsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : AnalyticsHeartbeat200Response = apiInstance.botUndeleteSkill(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SkillsApi#botUndeleteSkill")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SkillsApi#botUndeleteSkill")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**AnalyticsHeartbeat200Response**](AnalyticsHeartbeat200Response.md)

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

