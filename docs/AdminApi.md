# AdminApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**affiliatesAdminApproveAffiliate**](AdminApi.md#affiliatesAdminApproveAffiliate) | **POST** /v1/admin/affiliates/{id}/approve | Approve an affiliate and mint its code |
| [**affiliatesAdminListAffiliates**](AdminApi.md#affiliatesAdminListAffiliates) | **GET** /v1/admin/affiliates | List all affiliates |
| [**affiliatesAdminPayoutAffiliate**](AdminApi.md#affiliatesAdminPayoutAffiliate) | **POST** /v1/admin/affiliates/{id}/payout | Record a payout |
| [**affiliatesAdminSuspendAffiliate**](AdminApi.md#affiliatesAdminSuspendAffiliate) | **POST** /v1/admin/affiliates/{id}/suspend | Suspend an affiliate |
| [**affiliatesAdminSweepAffiliates**](AdminApi.md#affiliatesAdminSweepAffiliates) | **POST** /v1/admin/affiliates/sweep | Run the accrual sweep |
| [**analyticsAdminListUsers**](AdminApi.md#analyticsAdminListUsers) | **GET** /v1/analytics/admin/users | List all users (admin only) |
| [**analyticsAdminListWebsites**](AdminApi.md#analyticsAdminListWebsites) | **GET** /v1/analytics/admin/websites | List all websites for a user (admin only) |
| [**authorsAdminApproveAuthor**](AdminApi.md#authorsAdminApproveAuthor) | **POST** /v1/admin/authors/{id}/approve | Approve an author |
| [**authorsAdminListAuthors**](AdminApi.md#authorsAdminListAuthors) | **GET** /v1/admin/authors | List all authors |
| [**authorsAdminPayoutAuthor**](AdminApi.md#authorsAdminPayoutAuthor) | **POST** /v1/admin/authors/{id}/payout | Record a payout |
| [**authorsAdminSuspendAuthor**](AdminApi.md#authorsAdminSuspendAuthor) | **POST** /v1/admin/authors/{id}/suspend | Suspend an author |
| [**authorsAdminSweepAuthors**](AdminApi.md#authorsAdminSweepAuthors) | **POST** /v1/admin/authors/sweep | Run accrual sweep |
| [**kmsGetServerConfig**](AdminApi.md#kmsGetServerConfig) | **GET** /v1/kms/admin/config | Get server configuration |
| [**kmsUpdateServerConfig**](AdminApi.md#kmsUpdateServerConfig) | **PATCH** /v1/kms/admin/config | Update server configuration |
| [**referralsAdminListReferrals**](AdminApi.md#referralsAdminListReferrals) | **GET** /v1/admin/referrals | List every referral with a fleet summary (global-admin) |
| [**referralsAdminSweepReferrals**](AdminApi.md#referralsAdminSweepReferrals) | **POST** /v1/admin/referrals/sweep | Qualify-check every pending referral (global-admin) |
| [**s3AdminInfo**](AdminApi.md#s3AdminInfo) | **GET** /v1/s3/admin/info | Server information |
| [**s3AdminUsage**](AdminApi.md#s3AdminUsage) | **GET** /v1/s3/admin/usage | Storage usage |
| [**s3CreateServiceAccount**](AdminApi.md#s3CreateServiceAccount) | **POST** /v1/s3/admin/service-accounts | Create a service account |
| [**s3ListServiceAccounts**](AdminApi.md#s3ListServiceAccounts) | **GET** /v1/s3/admin/service-accounts | List service accounts |


<a id="affiliatesAdminApproveAffiliate"></a>
# **affiliatesAdminApproveAffiliate**
> AffiliatesAdminAffiliateEnvelope affiliatesAdminApproveAffiliate(id, affiliatesApproveRequest)

Approve an affiliate and mint its code

Approves the affiliate and mints its code. The body may carry an explicit &#x60;code&#x60; override; else the requested vanity code; else a derived slug. Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | The affiliate id (e.g. `aff_<hex>`).
val affiliatesApproveRequest : AffiliatesApproveRequest =  // AffiliatesApproveRequest | 
try {
    val result : AffiliatesAdminAffiliateEnvelope = apiInstance.affiliatesAdminApproveAffiliate(id, affiliatesApproveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#affiliatesAdminApproveAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#affiliatesAdminApproveAffiliate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The affiliate id (e.g. &#x60;aff_&lt;hex&gt;&#x60;). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliatesApproveRequest** | [**AffiliatesApproveRequest**](AffiliatesApproveRequest.md)|  | [optional] |

### Return type

[**AffiliatesAdminAffiliateEnvelope**](AffiliatesAdminAffiliateEnvelope.md)

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

<a id="affiliatesAdminListAffiliates"></a>
# **affiliatesAdminListAffiliates**
> AffiliatesAdminListEnvelope affiliatesAdminListAffiliates(limit)

List all affiliates

Returns every affiliate (org exposed) plus a fleet summary. Global-admin only. Wrapped in the admin &#x60;{ status, msg, data }&#x60; envelope. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val limit : kotlin.Int = 56 // kotlin.Int | Max rows to return (default 500, max 1000).
try {
    val result : AffiliatesAdminListEnvelope = apiInstance.affiliatesAdminListAffiliates(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#affiliatesAdminListAffiliates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#affiliatesAdminListAffiliates")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max rows to return (default 500, max 1000). | [optional] [default to 500] |

### Return type

[**AffiliatesAdminListEnvelope**](AffiliatesAdminListEnvelope.md)

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

<a id="affiliatesAdminPayoutAffiliate"></a>
# **affiliatesAdminPayoutAffiliate**
> AffiliatesAdminPayoutEnvelope affiliatesAdminPayoutAffiliate(id, affiliatesPayoutRequest)

Record a payout

Records a payout of accrued commission. A &#x60;credits&#x60; method issues a commerce grant into the affiliate&#39;s wallet; a cash method (wire/paypal/…) is record-only. The amount can never exceed pending (accrued − paid), reserved atomically before any grant. Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | The affiliate id (e.g. `aff_<hex>`).
val affiliatesPayoutRequest : AffiliatesPayoutRequest =  // AffiliatesPayoutRequest | 
try {
    val result : AffiliatesAdminPayoutEnvelope = apiInstance.affiliatesAdminPayoutAffiliate(id, affiliatesPayoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#affiliatesAdminPayoutAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#affiliatesAdminPayoutAffiliate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The affiliate id (e.g. &#x60;aff_&lt;hex&gt;&#x60;). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **affiliatesPayoutRequest** | [**AffiliatesPayoutRequest**](AffiliatesPayoutRequest.md)|  | |

### Return type

[**AffiliatesAdminPayoutEnvelope**](AffiliatesAdminPayoutEnvelope.md)

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

<a id="affiliatesAdminSuspendAffiliate"></a>
# **affiliatesAdminSuspendAffiliate**
> AffiliatesAdminAffiliateEnvelope affiliatesAdminSuspendAffiliate(id)

Suspend an affiliate

Suspends the affiliate. Global-admin only.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | The affiliate id (e.g. `aff_<hex>`).
try {
    val result : AffiliatesAdminAffiliateEnvelope = apiInstance.affiliatesAdminSuspendAffiliate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#affiliatesAdminSuspendAffiliate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#affiliatesAdminSuspendAffiliate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The affiliate id (e.g. &#x60;aff_&lt;hex&gt;&#x60;). | |

### Return type

[**AffiliatesAdminAffiliateEnvelope**](AffiliatesAdminAffiliateEnvelope.md)

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

<a id="affiliatesAdminSweepAffiliates"></a>
# **affiliatesAdminSweepAffiliates**
> AffiliatesAdminSweepEnvelope affiliatesAdminSweepAffiliates()

Run the accrual sweep

The periodic accrual path (cron/o11y hits it, or an operator on demand). It folds over every approved affiliate&#39;s referred orgs and accrues this period&#39;s commission, at-most-once per period. Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : AffiliatesAdminSweepEnvelope = apiInstance.affiliatesAdminSweepAffiliates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#affiliatesAdminSweepAffiliates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#affiliatesAdminSweepAffiliates")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AffiliatesAdminSweepEnvelope**](AffiliatesAdminSweepEnvelope.md)

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

<a id="analyticsAdminListUsers"></a>
# **analyticsAdminListUsers**
> kotlin.collections.List&lt;AnalyticsAdminListUsers200ResponseInner&gt; analyticsAdminListUsers(page, pageSize, orderBy, search)

List all users (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsAdminListUsers200ResponseInner> = apiInstance.analyticsAdminListUsers(page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#analyticsAdminListUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#analyticsAdminListUsers")
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

[**kotlin.collections.List&lt;AnalyticsAdminListUsers200ResponseInner&gt;**](AnalyticsAdminListUsers200ResponseInner.md)

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

<a id="analyticsAdminListWebsites"></a>
# **analyticsAdminListWebsites**
> kotlin.collections.List&lt;AnalyticsWebsite&gt; analyticsAdminListWebsites(userId, includeOwnedTeams, includeAllTeams, page, pageSize, orderBy, search)

List all websites for a user (admin only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val includeOwnedTeams : kotlin.String = includeOwnedTeams_example // kotlin.String | 
val includeAllTeams : kotlin.String = includeAllTeams_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsWebsite> = apiInstance.analyticsAdminListWebsites(userId, includeOwnedTeams, includeAllTeams, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#analyticsAdminListWebsites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#analyticsAdminListWebsites")
    e.printStackTrace()
}
```

### Parameters
| **userId** | **java.util.UUID**|  | |
| **includeOwnedTeams** | **kotlin.String**|  | [optional] |
| **includeAllTeams** | **kotlin.String**|  | [optional] |
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

<a id="authorsAdminApproveAuthor"></a>
# **authorsAdminApproveAuthor**
> AuthorsAdminAuthorEnvelope authorsAdminApproveAuthor(id, authorsApproveRequest)

Approve an author

Admits an author to earning. An optional &#x60;{shareBps}&#x60; body overrides the royalty share (0–10000 basis points). Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | Author id (e.g. aut_...).
val authorsApproveRequest : AuthorsApproveRequest =  // AuthorsApproveRequest | 
try {
    val result : AuthorsAdminAuthorEnvelope = apiInstance.authorsAdminApproveAuthor(id, authorsApproveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#authorsAdminApproveAuthor")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#authorsAdminApproveAuthor")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Author id (e.g. aut_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorsApproveRequest** | [**AuthorsApproveRequest**](AuthorsApproveRequest.md)|  | [optional] |

### Return type

[**AuthorsAdminAuthorEnvelope**](AuthorsAdminAuthorEnvelope.md)

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

<a id="authorsAdminListAuthors"></a>
# **authorsAdminListAuthors**
> AuthorsAdminListEnvelope authorsAdminListAuthors(limit)

List all authors

Every author (org exposed) plus a fleet summary. Global-admin only.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val limit : kotlin.Int = 56 // kotlin.Int | Max rows (default 500, capped at 1000).
try {
    val result : AuthorsAdminListEnvelope = apiInstance.authorsAdminListAuthors(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#authorsAdminListAuthors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#authorsAdminListAuthors")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max rows (default 500, capped at 1000). | [optional] [default to 500] |

### Return type

[**AuthorsAdminListEnvelope**](AuthorsAdminListEnvelope.md)

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

<a id="authorsAdminPayoutAuthor"></a>
# **authorsAdminPayoutAuthor**
> AuthorsAdminPayoutEnvelope authorsAdminPayoutAuthor(id, authorsPayoutRequest)

Record a payout

Records a payout of accrued royalty. A &#x60;credits&#x60; method issues a commerce grant into the author&#39;s wallet; a cash method (wire, paypal, check, …) is record-only. The amount can never exceed pending (accrued − paid), reserved atomically before any grant. Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | Author id (e.g. aut_...).
val authorsPayoutRequest : AuthorsPayoutRequest =  // AuthorsPayoutRequest | 
try {
    val result : AuthorsAdminPayoutEnvelope = apiInstance.authorsAdminPayoutAuthor(id, authorsPayoutRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#authorsAdminPayoutAuthor")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#authorsAdminPayoutAuthor")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Author id (e.g. aut_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **authorsPayoutRequest** | [**AuthorsPayoutRequest**](AuthorsPayoutRequest.md)|  | |

### Return type

[**AuthorsAdminPayoutEnvelope**](AuthorsAdminPayoutEnvelope.md)

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

<a id="authorsAdminSuspendAuthor"></a>
# **authorsAdminSuspendAuthor**
> AuthorsAdminAuthorEnvelope authorsAdminSuspendAuthor(id)

Suspend an author

Suspends an author. Global-admin only.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val id : kotlin.String = id_example // kotlin.String | Author id (e.g. aut_...).
try {
    val result : AuthorsAdminAuthorEnvelope = apiInstance.authorsAdminSuspendAuthor(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#authorsAdminSuspendAuthor")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#authorsAdminSuspendAuthor")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Author id (e.g. aut_...). | |

### Return type

[**AuthorsAdminAuthorEnvelope**](AuthorsAdminAuthorEnvelope.md)

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

<a id="authorsAdminSweepAuthors"></a>
# **authorsAdminSweepAuthors**
> AuthorsAdminSweepEnvelope authorsAdminSweepAuthors()

Run accrual sweep

The periodic accrual path. Folds over every approved author&#39;s distinct deploying orgs and accrues this period&#39;s royalty, at-most-once per period. Global-admin only. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : AuthorsAdminSweepEnvelope = apiInstance.authorsAdminSweepAuthors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#authorsAdminSweepAuthors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#authorsAdminSweepAuthors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AuthorsAdminSweepEnvelope**](AuthorsAdminSweepEnvelope.md)

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

<a id="kmsGetServerConfig"></a>
# **kmsGetServerConfig**
> KmsGetServerConfig200Response kmsGetServerConfig()

Get server configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : KmsGetServerConfig200Response = apiInstance.kmsGetServerConfig()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#kmsGetServerConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#kmsGetServerConfig")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsGetServerConfig200Response**](KmsGetServerConfig200Response.md)

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

<a id="kmsUpdateServerConfig"></a>
# **kmsUpdateServerConfig**
> kotlin.Any kmsUpdateServerConfig(kmsUpdateServerConfigRequest)

Update server configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val kmsUpdateServerConfigRequest : KmsUpdateServerConfigRequest =  // KmsUpdateServerConfigRequest | 
try {
    val result : kotlin.Any = apiInstance.kmsUpdateServerConfig(kmsUpdateServerConfigRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#kmsUpdateServerConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#kmsUpdateServerConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateServerConfigRequest** | [**KmsUpdateServerConfigRequest**](KmsUpdateServerConfigRequest.md)|  | |

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

<a id="referralsAdminListReferrals"></a>
# **referralsAdminListReferrals**
> ReferralsAdminListEnvelope referralsAdminListReferrals(limit)

List every referral with a fleet summary (global-admin)

Returns every referral (both orgs exposed) plus a fleet summary. Global-admin only. Wrapped in the &#x60;{ status, msg, data }&#x60; admin envelope. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val limit : kotlin.Int = 56 // kotlin.Int | Max rows to return. Defaults to 500 when absent/invalid/<=0; capped at 1000. 
try {
    val result : ReferralsAdminListEnvelope = apiInstance.referralsAdminListReferrals(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#referralsAdminListReferrals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#referralsAdminListReferrals")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Max rows to return. Defaults to 500 when absent/invalid/&lt;&#x3D;0; capped at 1000.  | [optional] [default to 500] |

### Return type

[**ReferralsAdminListEnvelope**](ReferralsAdminListEnvelope.md)

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

<a id="referralsAdminSweepReferrals"></a>
# **referralsAdminSweepReferrals**
> ReferralsAdminSweepEnvelope referralsAdminSweepReferrals()

Qualify-check every pending referral (global-admin)

The periodic qualify path (cron/operator on demand). Qualify-checks every pending referral (bounded to 500 per sweep) and grants the ones that now qualify. Global-admin only. Returns counts in the admin envelope. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : ReferralsAdminSweepEnvelope = apiInstance.referralsAdminSweepReferrals()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#referralsAdminSweepReferrals")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#referralsAdminSweepReferrals")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ReferralsAdminSweepEnvelope**](ReferralsAdminSweepEnvelope.md)

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

<a id="s3AdminInfo"></a>
# **s3AdminInfo**
> S3AdminInfo200Response s3AdminInfo()

Server information

Returns server version, storage capacity, and cluster status.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : S3AdminInfo200Response = apiInstance.s3AdminInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#s3AdminInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#s3AdminInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**S3AdminInfo200Response**](S3AdminInfo200Response.md)

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

<a id="s3AdminUsage"></a>
# **s3AdminUsage**
> S3UsageInfo s3AdminUsage()

Storage usage

Returns aggregate storage usage across all buckets.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : S3UsageInfo = apiInstance.s3AdminUsage()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#s3AdminUsage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#s3AdminUsage")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**S3UsageInfo**](S3UsageInfo.md)

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

<a id="s3CreateServiceAccount"></a>
# **s3CreateServiceAccount**
> S3ServiceAccount s3CreateServiceAccount(s3CreateServiceAccountRequest)

Create a service account

Create a service account with specific bucket access policies.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
val s3CreateServiceAccountRequest : S3CreateServiceAccountRequest =  // S3CreateServiceAccountRequest | 
try {
    val result : S3ServiceAccount = apiInstance.s3CreateServiceAccount(s3CreateServiceAccountRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#s3CreateServiceAccount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#s3CreateServiceAccount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3CreateServiceAccountRequest** | [**S3CreateServiceAccountRequest**](S3CreateServiceAccountRequest.md)|  | |

### Return type

[**S3ServiceAccount**](S3ServiceAccount.md)

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

<a id="s3ListServiceAccounts"></a>
# **s3ListServiceAccounts**
> S3ListServiceAccounts200Response s3ListServiceAccounts()

List service accounts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AdminApi()
try {
    val result : S3ListServiceAccounts200Response = apiInstance.s3ListServiceAccounts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#s3ListServiceAccounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#s3ListServiceAccounts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**S3ListServiceAccounts200Response**](S3ListServiceAccounts200Response.md)

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

