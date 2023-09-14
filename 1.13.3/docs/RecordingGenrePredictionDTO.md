# SongtradrApiClientRuby::RecordingGenrePredictionDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **genre_type** | **String** |  |  |
| **probability** | **Float** |  |  |
| **genre** | [**GenreMinimalDTO**](GenreMinimalDTO.md) |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingGenrePredictionDTO.new(
  genre_type: null,
  probability: null,
  genre: null
)
```

