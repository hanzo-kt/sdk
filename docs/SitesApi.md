# SitesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**projectsBuildSite**](SitesApi.md#projectsBuildSite) | **POST** /v1/sites | Build a site from a brief and deploy it |
| [**projectsDeploySite**](SitesApi.md#projectsDeploySite) | **POST** /v1/sites/deploy | Deploy a raw file manifest |
| [**projectsListSites**](SitesApi.md#projectsListSites) | **GET** /v1/sites | List the org&#39;s live sites |


<a id="projectsBuildSite"></a>
# **projectsBuildSite**
> ProjectsSiteDeployResult projectsBuildSite(projectsBuildSiteRequest)

Build a site from a brief and deploy it

Generate a self-contained, mobile-responsive static site from a natural-language &#x60;brief&#x60; (one inference call), then deploy it through the one publish core. Writes into the SAME org-scoped projects store as &#x60;/v1/projects&#x60;: it ensures a &#x60;project&#x60; (framework &#x60;static&#x60;) for the resolved slug and records a &#x60;deployment&#x60;. &#x60;/v1/sites&#x60; is the brief-build/raw-manifest entrypoint; &#x60;/v1/projects/{slug}/deploy&#x60; is the artifact/git entrypoint — one store, one publish core, not a second copy of project state. The brief is capped at 8 KiB. Responds &#x60;200&#x60; with the published-site result. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SitesApi()
val projectsBuildSiteRequest : ProjectsBuildSiteRequest =  // ProjectsBuildSiteRequest | 
try {
    val result : ProjectsSiteDeployResult = apiInstance.projectsBuildSite(projectsBuildSiteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SitesApi#projectsBuildSite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SitesApi#projectsBuildSite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsBuildSiteRequest** | [**ProjectsBuildSiteRequest**](ProjectsBuildSiteRequest.md)|  | |

### Return type

[**ProjectsSiteDeployResult**](ProjectsSiteDeployResult.md)

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

<a id="projectsDeploySite"></a>
# **projectsDeploySite**
> ProjectsSiteDeployResult projectsDeploySite(projectsDeploySiteRequest)

Deploy a raw file manifest

Deploy a caller-supplied file manifest (the same &#x60;{path, content}&#x60; shape the brief build emits) through the one publish core. Every file passes the same guards as the brief build: index.html required at the root; absolute and traversal paths rejected; a mobile viewport tag injected into HTML when absent. Writes into the SAME org-scoped projects store as &#x60;/v1/projects&#x60;: it ensures a &#x60;project&#x60; (framework &#x60;static&#x60;) for the resolved slug and records a &#x60;deployment&#x60;. &#x60;/v1/sites&#x60; is the brief-build/raw-manifest entrypoint; &#x60;/v1/projects/{slug}/deploy&#x60; is the artifact/git entrypoint — one store, one publish core, not a second copy of project state. Responds &#x60;200&#x60; with the published-site result. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SitesApi()
val projectsDeploySiteRequest : ProjectsDeploySiteRequest =  // ProjectsDeploySiteRequest | 
try {
    val result : ProjectsSiteDeployResult = apiInstance.projectsDeploySite(projectsDeploySiteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SitesApi#projectsDeploySite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SitesApi#projectsDeploySite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsDeploySiteRequest** | [**ProjectsDeploySiteRequest**](ProjectsDeploySiteRequest.md)|  | |

### Return type

[**ProjectsSiteDeployResult**](ProjectsSiteDeployResult.md)

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

<a id="projectsListSites"></a>
# **projectsListSites**
> kotlin.collections.List&lt;ProjectsSite&gt; projectsListSites()

List the org&#39;s live sites

List the org&#39;s &#x60;live&#x60; projects as sites at their canonical live URL &#x60;https://&lt;slug&gt;.&lt;apex&gt;&#x60;. Reads the SAME org-scoped projects store as &#x60;/v1/projects&#x60;; a project that is not &#x60;live&#x60; is omitted. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SitesApi()
try {
    val result : kotlin.collections.List<ProjectsSite> = apiInstance.projectsListSites()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SitesApi#projectsListSites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SitesApi#projectsListSites")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProjectsSite&gt;**](ProjectsSite.md)

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

