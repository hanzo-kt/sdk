
# DbRestoreBranchRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **sourceBranchId** | **kotlin.String** |  |  [optional] |
| **sourceLsn** | **kotlin.String** | Restore to this LSN |  [optional] |
| **sourceTimestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Restore to this point in time |  [optional] |
| **preserveUnderName** | **kotlin.String** | Preserve current state under this name before restoring |  [optional] |



