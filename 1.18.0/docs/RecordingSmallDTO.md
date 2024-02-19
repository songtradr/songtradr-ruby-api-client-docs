# SongtradrApiClientRuby::RecordingSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **tracks** | [**Array&lt;TrackDTO&gt;**](TrackDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingSmallDTO.new(
  duration: null,
  titles: null,
  tracks: null,
  isrc: null,
  parties: null
)
```

