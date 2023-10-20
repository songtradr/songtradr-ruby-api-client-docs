# SongtradrApiClientRuby::RecordingMinimalWithTaggramsDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **isrc** | **String** |  |  |
| **timestamps** | **Array&lt;Float&gt;** | Points in time in seconds. Each value refers to the taggrams values of the same index. | [optional] |
| **taggrams** | [**Array&lt;TaggramDTO&gt;**](TaggramDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingMinimalWithTaggramsDTO.new(
  isrc: null,
  timestamps: null,
  taggrams: null
)
```

