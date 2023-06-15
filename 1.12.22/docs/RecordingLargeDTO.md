# SongtradrApiClientRuby::RecordingLargeDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **tracks** | [**Array&lt;TrackToMediumProductDTO&gt;**](TrackToMediumProductDTO.md) |  | [optional] |
| **musical_features** | [**MusicalFeaturesDTO**](MusicalFeaturesDTO.md) |  | [optional] |
| **pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] |
| **genre_predictions** | [**Array&lt;RecordingGenrePredictionDTO&gt;**](RecordingGenrePredictionDTO.md) |  | [optional] |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreDTO&gt;**](GenreDTO.md) |  | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |
| **tags** | [**Array&lt;RecordingTagSmallDTO&gt;**](RecordingTagSmallDTO.md) |  | [optional] |
| **spotify_id** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingLargeDTO.new(
  duration: null,
  tracks: null,
  musical_features: null,
  pline: null,
  genre_predictions: null,
  parties: null,
  genres: null,
  language_of_performance: null,
  titles: null,
  isrc: null,
  tags: null,
  spotify_id: null
)
```

