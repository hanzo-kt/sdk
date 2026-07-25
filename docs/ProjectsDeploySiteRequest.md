
# ProjectsDeploySiteRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **files** | [**kotlin.collections.List&lt;ProjectsSiteFile&gt;**](ProjectsSiteFile.md) | Site files (required, non-empty); index.html must be present at the root. |  |
| **slug** | **kotlin.String** | Target project slug; derived from name (or minted \&quot;site-&lt;token&gt;\&quot;) when omitted. |  [optional] |
| **name** | **kotlin.String** | Display name; defaults to \&quot;Site\&quot;. |  [optional] |



