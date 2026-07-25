# DeploymentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mlDeployModel**](DeploymentsApi.md#mlDeployModel) | **POST** /v1/ml/deploy | Deploy a model |
| [**mlGetDeployment**](DeploymentsApi.md#mlGetDeployment) | **GET** /v1/ml/deployments/{deployment_id} | Get deployment details |
| [**mlListDeployments**](DeploymentsApi.md#mlListDeployments) | **GET** /v1/ml/deployments | List deployments |
| [**mlStopDeployment**](DeploymentsApi.md#mlStopDeployment) | **DELETE** /v1/ml/deployments/{deployment_id} | Stop a deployment |
| [**projectsCompleteDeployment**](DeploymentsApi.md#projectsCompleteDeployment) | **POST** /v1/projects/{slug}/deployments/{id}/complete | CI completion hook for a git deployment |
| [**projectsDeployProject**](DeploymentsApi.md#projectsDeployProject) | **POST** /v1/projects/{slug}/deploy | Deploy a project to the S3 origin |
| [**projectsGetDeployment**](DeploymentsApi.md#projectsGetDeployment) | **GET** /v1/projects/{slug}/deployments/{id} | Get a deployment |
| [**projectsListDeployments**](DeploymentsApi.md#projectsListDeployments) | **GET** /v1/projects/{slug}/deployments | List deployments for a project |
| [**projectsPurgeProject**](DeploymentsApi.md#projectsPurgeProject) | **POST** /v1/projects/{slug}/purge | Purge the site&#39;s edge cache |


<a id="mlDeployModel"></a>
# **mlDeployModel**
> MlDeployment mlDeployModel(mlDeployModelRequest)

Deploy a model

Deploy a model from the registry to Hanzo Cloud.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val mlDeployModelRequest : MlDeployModelRequest = {"model_id":"my-finetune","model_version":"v3","runtime":"vllm","gpu":"a100","replicas":2,"environment":"production"} // MlDeployModelRequest | 
try {
    val result : MlDeployment = apiInstance.mlDeployModel(mlDeployModelRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#mlDeployModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#mlDeployModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlDeployModelRequest** | [**MlDeployModelRequest**](MlDeployModelRequest.md)|  | |

### Return type

[**MlDeployment**](MlDeployment.md)

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

<a id="mlGetDeployment"></a>
# **mlGetDeployment**
> MlDeployment mlGetDeployment(deploymentId)

Get deployment details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val deploymentId : kotlin.String = deploymentId_example // kotlin.String | 
try {
    val result : MlDeployment = apiInstance.mlGetDeployment(deploymentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#mlGetDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#mlGetDeployment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deploymentId** | **kotlin.String**|  | |

### Return type

[**MlDeployment**](MlDeployment.md)

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

<a id="mlListDeployments"></a>
# **mlListDeployments**
> MlListDeployments200Response mlListDeployments(environment, status)

List deployments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val environment : kotlin.String = environment_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
try {
    val result : MlListDeployments200Response = apiInstance.mlListDeployments(environment, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#mlListDeployments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#mlListDeployments")
    e.printStackTrace()
}
```

### Parameters
| **environment** | **kotlin.String**|  | [optional] [enum: dev, staging, production] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] [enum: deploying, active, failed, stopped] |

### Return type

[**MlListDeployments200Response**](MlListDeployments200Response.md)

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

<a id="mlStopDeployment"></a>
# **mlStopDeployment**
> mlStopDeployment(deploymentId)

Stop a deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val deploymentId : kotlin.String = deploymentId_example // kotlin.String | 
try {
    apiInstance.mlStopDeployment(deploymentId)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#mlStopDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#mlStopDeployment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deploymentId** | **kotlin.String**|  | |

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

<a id="projectsCompleteDeployment"></a>
# **projectsCompleteDeployment**
> ProjectsDeployment projectsCompleteDeployment(slug, id, projectsCompleteDeploymentRequest)

CI completion hook for a git deployment

After CI syncs the built site to the S3 origin it flips the &#x60;queued&#x60; deployment to &#x60;live&#x60; (or &#x60;error&#x60;). &#x60;status&#x60; must be &#x60;live&#x60; or &#x60;error&#x60;. When &#x60;liveUrl&#x60; is omitted on a live completion it defaults to the project&#39;s canonical live URL. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
val id : kotlin.String = id_example // kotlin.String | Deployment id (e.g. dep_...).
val projectsCompleteDeploymentRequest : ProjectsCompleteDeploymentRequest =  // ProjectsCompleteDeploymentRequest | 
try {
    val result : ProjectsDeployment = apiInstance.projectsCompleteDeployment(slug, id, projectsCompleteDeploymentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#projectsCompleteDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#projectsCompleteDeployment")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |
| **id** | **kotlin.String**| Deployment id (e.g. dep_...). | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsCompleteDeploymentRequest** | [**ProjectsCompleteDeploymentRequest**](ProjectsCompleteDeploymentRequest.md)|  | |

### Return type

[**ProjectsDeployment**](ProjectsDeployment.md)

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

<a id="projectsDeployProject"></a>
# **projectsDeployProject**
> ProjectsDeployment projectsDeployProject(slug, projectsGitDeployRequest)

Deploy a project to the S3 origin

The artifact/git entrypoint. Two modes on one endpoint, selected by Content-Type; both funnel through the one publish core.  - Artifact (default): the request body is a zip or tar(.gz) of the BUILT   site (index.html at the root, or inside a single wrapper directory),   sent as a raw body or a multipart file. It is unpacked to the S3 origin   under &#x60;&lt;org&gt;/&lt;slug&gt;/&#x60;, marked public-read, recorded as a &#x60;live&#x60;   deployment, and served at &#x60;https://&lt;slug&gt;.&lt;apex&gt;&#x60;. Responds &#x60;200&#x60; with   the finalized deployment. - Git (&#x60;Content-Type: application/json&#x60;, body &#x60;{\&quot;source\&quot;:\&quot;git\&quot;, ...}&#x60;):   records a &#x60;queued&#x60; deployment and responds &#x60;202&#x60;. CI builds the linked   repo, syncs &#x60;dist/&#x60; to the same prefix, then calls the completion hook   to flip it &#x60;live&#x60;. Requires the project to have a linked repo. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
val projectsGitDeployRequest : ProjectsGitDeployRequest =  // ProjectsGitDeployRequest | 
try {
    val result : ProjectsDeployment = apiInstance.projectsDeployProject(slug, projectsGitDeployRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#projectsDeployProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#projectsDeployProject")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsGitDeployRequest** | [**ProjectsGitDeployRequest**](ProjectsGitDeployRequest.md)|  | |

### Return type

[**ProjectsDeployment**](ProjectsDeployment.md)

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

<a id="projectsGetDeployment"></a>
# **projectsGetDeployment**
> ProjectsDeployment projectsGetDeployment(slug, id)

Get a deployment

Read one deployment of a project by id.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
val id : kotlin.String = id_example // kotlin.String | Deployment id (e.g. dep_...).
try {
    val result : ProjectsDeployment = apiInstance.projectsGetDeployment(slug, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#projectsGetDeployment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#projectsGetDeployment")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Deployment id (e.g. dep_...). | |

### Return type

[**ProjectsDeployment**](ProjectsDeployment.md)

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

<a id="projectsListDeployments"></a>
# **projectsListDeployments**
> kotlin.collections.List&lt;ProjectsDeployment&gt; projectsListDeployments(slug)

List deployments for a project

List the project&#39;s deployments, newest version first.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
try {
    val result : kotlin.collections.List<ProjectsDeployment> = apiInstance.projectsListDeployments(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#projectsListDeployments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#projectsListDeployments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |

### Return type

[**kotlin.collections.List&lt;ProjectsDeployment&gt;**](ProjectsDeployment.md)

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

<a id="projectsPurgeProject"></a>
# **projectsPurgeProject**
> ProjectsProject projectsPurgeProject(slug)

Purge the site&#39;s edge cache

Flush the site&#39;s edge cache without redeploying: invalidate the edge cache-tag &#x60;site-&lt;org&gt;-&lt;slug&gt;&#x60;, then stamp &#x60;lastPurgeAt&#x60; (unix seconds). The S3 origin and the deployment history are untouched — only cached copies at the edge are dropped, so the next request re-fetches the current artifact from origin. Idempotent. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DeploymentsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
try {
    val result : ProjectsProject = apiInstance.projectsPurgeProject(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeploymentsApi#projectsPurgeProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeploymentsApi#projectsPurgeProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |

### Return type

[**ProjectsProject**](ProjectsProject.md)

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

