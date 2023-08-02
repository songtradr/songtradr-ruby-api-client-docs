# SongtradrApiClientRuby::PlaylistLargeDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **state** | **String** |  | [optional] |
| **usages** | [**Array&lt;UsageDTO&gt;**](UsageDTO.md) |  | [optional] |
| **description** | **String** |  | [optional] |
| **songtradr_playlist_guid** | **String** |  | [optional] |
| **asset_url** | **String** |  | [optional] |
| **pretzel_tier** | **String** |  | [optional] |
| **usage** | **String** |  | [optional] |
| **tracks** | [**Array&lt;RecordingPlaylistDTO&gt;**](RecordingPlaylistDTO.md) |  | [optional] |
| **created** | **Time** |  | [optional] |
| **updated** | **Time** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::PlaylistLargeDTO.new(
  name: null,
  state: null,
  usages: null,
  description: null,
  songtradr_playlist_guid: null,
  asset_url: null,
  pretzel_tier: null,
  usage: null,
  tracks: null,
  created: null,
  updated: null
)
```

