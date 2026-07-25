
# AuthorsAuthorDashboard

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **isAuthor** | **kotlin.Boolean** |  |  [optional] |
| **id** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **githubLogin** | **kotlin.String** |  |  [optional] |
| **verified** | **kotlin.Boolean** |  |  [optional] |
| **verifyCode** | **kotlin.String** |  |  [optional] |
| **verifyFile** | **kotlin.String** |  |  [optional] |
| **verifySnippet** | **kotlin.String** | The hanzo.json body to place on the default branch for file verification. |  [optional] |
| **shareBps** | **kotlin.Long** |  |  [optional] |
| **badgeBase** | **kotlin.String** |  |  [optional] |
| **repos** | [**kotlin.collections.List&lt;AuthorsRepoView&gt;**](AuthorsRepoView.md) |  |  [optional] |
| **deploys** | [**kotlin.collections.List&lt;AuthorsDeployView&gt;**](AuthorsDeployView.md) |  |  [optional] |
| **accruedCents** | **kotlin.Long** |  |  [optional] |
| **pendingCents** | **kotlin.Long** |  |  [optional] |
| **paidCents** | **kotlin.Long** |  |  [optional] |
| **payouts** | [**kotlin.collections.List&lt;AuthorsPayoutView&gt;**](AuthorsPayoutView.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | connected, approved, suspended |



