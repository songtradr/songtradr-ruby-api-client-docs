# SongtradrApiClientRuby::RecordingMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **recording_party_entities** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreDTO&gt;**](GenreDTO.md) |  | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **tracks** | [**Array&lt;TrackDTO&gt;**](TrackDTO.md) |  | [optional] |
| **musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |
| **tags** | [**Array&lt;RecordingTagSmallDTO&gt;**](RecordingTagSmallDTO.md) |  | [optional] |
| **spotify_id** | **String** |  | [optional] |
| **genre_predictions** | [**Array&lt;RecordingGenrePredictionDTO&gt;**](RecordingGenrePredictionDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingMediumDTO.new(
  recording_party_entities: null,
  genres: null,
  language_of_performance: null,
  release_date: null,
  titles: null,
  tracks: null,
  musical_features: null,
  isrc: null,
  tags: null,
  spotify_id: null,
  genre_predictions: null
)
```

