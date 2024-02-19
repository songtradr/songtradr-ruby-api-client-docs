# SongtradrApiClientRuby::RecordingMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **genres** | [**Array&lt;GenreDTO&gt;**](GenreDTO.md) |  | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **tracks** | [**Array&lt;TrackDTO&gt;**](TrackDTO.md) |  | [optional] |
| **musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |
| **recording_party_entities** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **spotify_id** | **String** |  | [optional] |
| **tags** | [**Array&lt;RecordingTagSmallDTO&gt;**](RecordingTagSmallDTO.md) |  | [optional] |
| **genre_predictions** | [**Array&lt;RecordingGenrePredictionDTO&gt;**](RecordingGenrePredictionDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingMediumDTO.new(
  genres: null,
  language_of_performance: null,
  release_date: null,
  titles: null,
  tracks: null,
  musical_features: null,
  isrc: null,
  recording_party_entities: null,
  spotify_id: null,
  tags: null,
  genre_predictions: null
)
```

