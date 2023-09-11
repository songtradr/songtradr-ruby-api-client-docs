# SongtradrApiClientRuby::PlaylistLargeDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **state** | **String** |  | [optional] |
| **songtradr_playlist_guid** | **String** |  | [optional] |
| **pretzel_tier** | **String** |  | [optional] |
| **asset_url** | **String** |  | [optional] |
| **usage** | **String** |  | [optional] |
| **usages** | [**Array&lt;UsageDTO&gt;**](UsageDTO.md) |  | [optional] |
| **tracks** | [**Array&lt;RecordingPlaylistDTO&gt;**](RecordingPlaylistDTO.md) |  | [optional] |
| **created** | **Time** |  | [optional] |
| **updated** | **Time** |  | [optional] |
| **description** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::PlaylistLargeDTO.new(
  name: null,
  state: null,
  songtradr_playlist_guid: null,
  pretzel_tier: null,
  asset_url: null,
  usage: null,
  usages: null,
  tracks: null,
  created: null,
  updated: null,
  description: null
)
```

