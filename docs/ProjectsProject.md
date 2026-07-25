
# ProjectsProject

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **org** | **kotlin.String** |  |  |
| **slug** | **kotlin.String** |  |  |
| **name** | **kotlin.String** |  |  |
| **repo** | [**ProjectsRepoRef**](ProjectsRepoRef.md) |  |  |
| **framework** | [**inline**](#Framework) | Build hint. |  |
| **status** | [**inline**](#Status) | Project lifecycle status. |  |
| **createdAt** | **kotlin.Long** |  |  |
| **updatedAt** | **kotlin.Long** |  |  |
| **description** | **kotlin.String** |  |  [optional] |
| **liveUrl** | **kotlin.String** | Canonical live URL, https://&lt;slug&gt;.&lt;apex&gt;. Set once deployed. |  [optional] |
| **bucket** | **kotlin.String** | S3-origin bucket holding the site. |  [optional] |
| **currentDeploymentId** | **kotlin.String** |  |  [optional] |
| **cacheControl** | **kotlin.String** | Per-project HTML/document Cache-Control policy applied at the S3 origin. |  [optional] |
| **lastPurgeAt** | **kotlin.Long** | Unix time (seconds) of the last edge cache-tag purge. |  [optional] |


<a id="Framework"></a>
## Enum: framework
| Name | Value |
| ---- | ----- |
| framework | static, vite, next, react, astro, svelte, vue, remix, nuxt, unity, unreal, godot |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | draft, building, live, error |



