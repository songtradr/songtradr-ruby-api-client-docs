# SongtradrApiClientRuby::PlaylistLargeDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **state** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |
| **usages** | [**Array&lt;UsageDTO&gt;**](UsageDTO.md) |  | [optional] |
| **created** | **Time** |  | [optional] |
| **updated** | **Time** |  | [optional] |
| **songtradr_playlist_guid** | **String** |  | [optional] |
| **tracks** | [**Array&lt;RecordingPlaylistDTO&gt;**](RecordingPlaylistDTO.md) |  | [optional] |
| **asset_url** | **String** |  | [optional] |
| **pretzel_tier** | **String** |  | [optional] |
| **usage** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::PlaylistLargeDTO.new(
  name: null,
  state: null,
  description: null,
  usages: null,
  created: null,
  updated: null,
  songtradr_playlist_guid: null,
  tracks: null,
  asset_url: null,
  pretzel_tier: null,
  usage: null
)
```

