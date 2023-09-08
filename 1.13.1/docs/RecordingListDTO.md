# SongtradrApiClientRuby::RecordingListDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **recordings** | [**Array&lt;RecordingMediumDTO&gt;**](RecordingMediumDTO.md) |  |  |
| **has_next_page** | **Boolean** |  |  |
| **current_page_number** | **Integer** |  |  |
| **total_results** | **Integer** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingListDTO.new(
  recordings: null,
  has_next_page: null,
  current_page_number: null,
  total_results: null
)
```

