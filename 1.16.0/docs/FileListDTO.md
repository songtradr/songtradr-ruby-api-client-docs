# SongtradrApiClientRuby::FileListDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **files** | [**Array&lt;FileDTO&gt;**](FileDTO.md) |  |  |
| **has_next_page** | **Boolean** |  |  |
| **current_page_number** | **Integer** |  |  |
| **total_results** | **Integer** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FileListDTO.new(
  files: null,
  has_next_page: null,
  current_page_number: null,
  total_results: null
)
```

