# SongtradrApiClientRuby::RecordingSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **isrc** | **String** |  |  |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingSmallDTO.new(
  duration: null,
  isrc: null,
  titles: null,
  parties: null
)
```

