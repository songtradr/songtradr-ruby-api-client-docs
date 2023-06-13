# SongtradrApiClientRuby::RecordingSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Integer** |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **parties** | [**Array&lt;RecordingPartyDTO&gt;**](RecordingPartyDTO.md) |  | [optional] |
| **isrc** | **String** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingSmallDTO.new(
  duration: null,
  titles: null,
  parties: null,
  isrc: null
)
```

