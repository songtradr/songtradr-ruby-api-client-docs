# SongtradrApiClientRuby::SavePlaylistDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **songtradr_playlist_guid** | **String** |  |  |
| **name** | **String** |  |  |
| **description** | **String** |  | [optional] |
| **state** | **String** |  |  |
| **asset_url** | **String** |  | [optional] |
| **pretzel_tier** | **String** |  | [optional] |
| **usage** | **String** |  | [optional] |
| **usages** | **Array&lt;String&gt;** |  |  |
| **recordings** | [**Array&lt;SaveRecordingPlaylistDTO&gt;**](SaveRecordingPlaylistDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::SavePlaylistDTO.new(
  songtradr_playlist_guid: null,
  name: null,
  description: null,
  state: null,
  asset_url: null,
  pretzel_tier: null,
  usage: null,
  usages: null,
  recordings: null
)
```

