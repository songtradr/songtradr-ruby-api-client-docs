# SongtradrApiClientRuby::RecordingLargeDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **spotify_id** | **String** |  | [optional] |
| **genre_predictions** | [**Array&lt;RecordingGenrePredictionDTO&gt;**](RecordingGenrePredictionDTO.md) |  | [optional] |
| **pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] |
| **tags** | [**Array&lt;RecordingTagSmallDTO&gt;**](RecordingTagSmallDTO.md) |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **tracks** | [**Array&lt;TrackToMediumProductDTO&gt;**](TrackToMediumProductDTO.md) |  | [optional] |
| **musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreDTO&gt;**](GenreDTO.md) |  | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **isrc** | **String** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingLargeDTO.new(
  duration: null,
  spotify_id: null,
  genre_predictions: null,
  pline: null,
  tags: null,
  titles: null,
  tracks: null,
  musical_features: null,
  parties: null,
  genres: null,
  language_of_performance: null,
  isrc: null
)
```

