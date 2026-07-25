
# ProjectsDeployment

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **projectId** | **kotlin.String** |  |  |
| **version** | **kotlin.Int** | Monotonic per project, 1-based. |  |
| **status** | [**inline**](#Status) | Deployment status. |  |
| **source** | [**inline**](#Source) | How the artifact was produced. |  |
| **files** | **kotlin.Int** |  |  |
| **bytes** | **kotlin.Long** |  |  |
| **createdAt** | **kotlin.Long** |  |  |
| **updatedAt** | **kotlin.Long** |  |  |
| **commit** | **kotlin.String** |  |  [optional] |
| **liveUrl** | **kotlin.String** | Canonical live URL, https://&lt;slug&gt;.&lt;apex&gt;. |  [optional] |
| **bucket** | **kotlin.String** | S3-origin bucket. |  [optional] |
| **prefix** | **kotlin.String** | S3-origin key prefix the site is served from (&lt;org&gt;/&lt;slug&gt;). |  [optional] |
| **message** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | queued, building, uploading, live, error |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | upload, generated, deploy, git |



