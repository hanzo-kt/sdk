
# ObserveStatusResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **product** | **kotlin.String** |  |  [optional] |
| **up** | **kotlin.Boolean** |  |  [optional] |
| **latencyMs** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Health-probe round trip; -1 when the probe did not complete. |  [optional] |
| **httpCode** | **kotlin.Int** | Health-probe status code (0 &#x3D; no response). |  [optional] |
| **scrapeUp** | **kotlin.Int** | VictoriaMetrics up{service}: 1/0, or null when no scrape target. |  [optional] |
| **probeUrl** | **kotlin.String** |  |  [optional] |
| **source** | [**inline**](#Source) | Which signal set &#x60;up&#x60;. |  [optional] |
| **checkedAt** | **kotlin.String** | RFC3339 timestamp (UTC). |  [optional] |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | probe, scrape, none |



