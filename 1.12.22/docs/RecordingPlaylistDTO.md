# SongtradrApiClientRuby::RecordingPlaylistDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **recording** | [**RecordingMediumDTO**](RecordingMediumDTO.md) |  | [optional] |
| **assigned_by_id** | **Integer** |  | [optional] |
| **sequence** | **Integer** |  | [optional] |
| **songtradr_track_guid** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingPlaylistDTO.new(
  recording: null,
  assigned_by_id: null,
  sequence: null,
  songtradr_track_guid: null
)
```

