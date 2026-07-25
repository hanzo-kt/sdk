
# ProjectsBuildSiteRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **brief** | **kotlin.String** | Natural-language description of the site to generate (required; capped at 8 KiB). |  |
| **slug** | **kotlin.String** | Target project slug; derived from name (or minted \&quot;site-&lt;token&gt;\&quot;) when omitted. |  [optional] |
| **name** | **kotlin.String** | Display name; defaults to the generated site name, else \&quot;Site\&quot;. |  [optional] |
| **model** | **kotlin.String** | Inference model override; empty selects the gateway default. |  [optional] |



