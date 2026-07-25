
# ReferralsMyReferralsResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **code** | **kotlin.String** | The caller org&#39;s stable referral code. |  [optional] |
| **link** | [**java.net.URI**](java.net.URI.md) | The share link, &#x60;&lt;linkBase&gt;/?ref&#x3D;&lt;code&gt;&#x60;. |  [optional] |
| **referrerBonusCents** | **kotlin.Long** | Bonus granted to the referrer on qualification (1000 &#x3D; $10). |  [optional] |
| **refereeBonusCents** | **kotlin.Long** | Bonus granted to the referee on qualification (500 &#x3D; $5). |  [optional] |
| **creditsEarnedCents** | **kotlin.Long** | Total credit earned across all of the caller&#39;s referrals. |  [optional] |
| **counts** | [**ReferralsStatusCounts**](ReferralsStatusCounts.md) |  |  [optional] |
| **referrals** | [**kotlin.collections.List&lt;ReferralsMyReferralView&gt;**](ReferralsMyReferralView.md) |  |  [optional] |



