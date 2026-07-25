
# AffiliatesGetMyAffiliate200Response

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **isAffiliate** | [**inline**](#IsAffiliate) |  |  [optional] |
| **defaultRateBps** | **kotlin.Long** | The default commission rate a new affiliate gets, in basis points (2000 &#x3D; 20%). |  [optional] |
| **id** | **kotlin.String** |  |  [optional] |
| **status** | [**AffiliatesAffiliateStatus**](AffiliatesAffiliateStatus.md) |  |  [optional] |
| **code** | **kotlin.String** | The minted affiliate code (empty until approved). |  [optional] |
| **requestedCode** | **kotlin.String** | The vanity code requested at apply, pending approval. |  [optional] |
| **link** | **kotlin.String** | The &#x60;?aff&#x60; referral link (empty until the affiliate has a code). |  [optional] |
| **rateBps** | **kotlin.Long** | Commission rate in basis points. |  [optional] |
| **referredCount** | **kotlin.Int** | Number of referred orgs attributed to this affiliate. |  [optional] |
| **accruedCents** | **kotlin.Long** | Lifetime commission accrued (USD cents). |  [optional] |
| **pendingCents** | **kotlin.Long** | Commission accrued but not yet paid (accrued − paid, never negative). |  [optional] |
| **paidCents** | **kotlin.Long** | Lifetime commission paid out (USD cents). |  [optional] |
| **payouts** | [**kotlin.collections.List&lt;AffiliatesPayout&gt;**](AffiliatesPayout.md) |  |  [optional] |


<a id="IsAffiliate"></a>
## Enum: isAffiliate
| Name | Value |
| ---- | ----- |
| isAffiliate | true |



