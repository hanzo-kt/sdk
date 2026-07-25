
# AffiliatesPayoutRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **amountCents** | **kotlin.Long** | Payout amount in USD cents (must be positive; cannot exceed pending commission). |  |
| **method** | **kotlin.String** | Payout method. &#x60;credits&#x60; issues a commerce grant; any other value (wire/paypal/check/…) is record-only. |  |
| **reference** | **kotlin.String** | Optional external reference for a cash payout. |  [optional] |



