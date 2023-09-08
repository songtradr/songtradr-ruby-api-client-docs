# SongtradrApiClientRuby::RecordingSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **isrc** | **String** |  |  |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingSmallDTO.new(
  duration: null,
  isrc: null,
  parties: null,
  titles: null
)
```

