# SongtradrApiClientRuby::RecordingPlaylistDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **recording** | [**RecordingMediumDTO**](RecordingMediumDTO.md) |  | [optional] |
| **songtradr_track_guid** | **String** |  | [optional] |
| **assigned_by_id** | **Integer** |  | [optional] |
| **sequence** | **Integer** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingPlaylistDTO.new(
  recording: null,
  songtradr_track_guid: null,
  assigned_by_id: null,
  sequence: null
)
```

