
# AuthorsPayoutRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **amountCents** | **kotlin.Long** | Payout amount in USD minor units (cents). Must be positive and not exceed pending. |  |
| **method** | **kotlin.String** | Payout method. &#39;credits&#39; issues a commerce grant; any other value (wire, paypal, check, …) is record-only. |  |
| **reference** | **kotlin.String** | Optional external reference for a cash disbursement. |  [optional] |



