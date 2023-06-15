# SongtradrApiClientRuby::RecordingMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] |
| **genre_predictions** | [**Array&lt;RecordingGenrePredictionDTO&gt;**](RecordingGenrePredictionDTO.md) |  | [optional] |
| **recording_party_entities** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreDTO&gt;**](GenreDTO.md) |  | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |
| **tags** | [**Array&lt;RecordingTagSmallDTO&gt;**](RecordingTagSmallDTO.md) |  | [optional] |
| **spotify_id** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingMediumDTO.new(
  musical_features: null,
  genre_predictions: null,
  recording_party_entities: null,
  genres: null,
  language_of_performance: null,
  release_date: null,
  titles: null,
  isrc: null,
  tags: null,
  spotify_id: null
)
```

