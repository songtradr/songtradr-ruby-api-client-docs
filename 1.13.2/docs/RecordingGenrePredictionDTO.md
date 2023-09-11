# SongtradrApiClientRuby::RecordingGenrePredictionDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **genre_type** | **String** |  |  |
| **genre** | [**GenreMinimalDTO**](GenreMinimalDTO.md) |  |  |
| **probability** | **Float** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingGenrePredictionDTO.new(
  genre_type: null,
  genre: null,
  probability: null
)
```

