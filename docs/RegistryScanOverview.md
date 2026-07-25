
# RegistryScanOverview

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **reportId** | **kotlin.String** |  |  [optional] |
| **scanStatus** | [**inline**](#ScanStatus) |  |  [optional] |
| **severity** | [**inline**](#Severity) |  |  [optional] |
| **startTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **endTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **completePercent** | **kotlin.Int** |  |  [optional] |
| **summary** | [**RegistryScanOverviewSummary**](RegistryScanOverviewSummary.md) |  |  [optional] |


<a id="ScanStatus"></a>
## Enum: scan_status
| Name | Value |
| ---- | ----- |
| scanStatus | Pending, Queued, Running, Success, Error, Stopped |


<a id="Severity"></a>
## Enum: severity
| Name | Value |
| ---- | ----- |
| severity | None, Low, Medium, High, Critical |



