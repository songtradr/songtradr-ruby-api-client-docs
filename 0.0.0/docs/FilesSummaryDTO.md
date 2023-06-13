# SongtradrApiClientRuby::FilesSummaryDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file_details_summary** | [**Array&lt;FieldSummaryDTO&gt;**](FieldSummaryDTO.md) |  | [optional] |
| **genre_summary** | [**Array&lt;GenresSummaryDTO&gt;**](GenresSummaryDTO.md) |  | [optional] |
| **tag_summary** | [**Array&lt;TagsSummaryDTO&gt;**](TagsSummaryDTO.md) |  | [optional] |
| **musical_features_summary** | [**Array&lt;FieldSummaryDTO&gt;**](FieldSummaryDTO.md) |  | [optional] |
| **total_files** | **Integer** |  |  |
| **bpm_min** | **Float** |  | [optional] |
| **bpm_max** | **Float** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FilesSummaryDTO.new(
  file_details_summary: null,
  genre_summary: null,
  tag_summary: null,
  musical_features_summary: null,
  total_files: null,
  bpm_min: null,
  bpm_max: null
)
```

