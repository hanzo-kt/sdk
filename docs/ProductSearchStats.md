
# ProductSearchStats

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **totalDocuments** | **kotlin.Long** | Total documents across all indexes. |  |
| **totalSearches** | **kotlin.Long** | Always 0 — Meilisearch keeps no query-history counters. |  |
| **totalSessions** | **kotlin.Long** | Always 0 — not derivable from the index. |  |
| **searchesPerDay** | [**kotlin.collections.List&lt;ProductDayCount&gt;**](ProductDayCount.md) | Always empty — no per-day query history is available. |  |



