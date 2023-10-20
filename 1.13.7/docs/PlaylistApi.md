# SongtradrApiClientRuby::PlaylistApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**all_playlists**](PlaylistApi.md#all_playlists) | **GET** /api/v1/playlist | All playlists. |
| [**create_or_update_playlist**](PlaylistApi.md#create_or_update_playlist) | **POST** /api/v1/playlist | Create and edit playlist. |
| [**curate_playlist**](PlaylistApi.md#curate_playlist) | **POST** /api/v1/playlist/{methodName} | Curate playlist. |
| [**delete_playlist**](PlaylistApi.md#delete_playlist) | **DELETE** /api/v1/playlist/{songtradrPlaylistGuid} | Delete playlist. |


## all_playlists

> <Array<PlaylistLargeDTO>> all_playlists(opts)

All playlists.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::PlaylistApi.new
opts = {
  include_recordings: true, # Boolean | Whether a playlist shall include recordings or not.
  ignore_usages: true, # Boolean | Whether a playlist shall include all songs regardless of their track usages.
  usage_filter_mode: 'any', # String | Whether a playlist recordings shall include all playlist usages or not.
  songtradr_playlist_guid: 'songtradr_playlist_guid_example' # String | 
}

begin
  # All playlists.
  result = api_instance.all_playlists(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->all_playlists: #{e}"
end
```

#### Using the all_playlists_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<PlaylistLargeDTO>>, Integer, Hash)> all_playlists_with_http_info(opts)

```ruby
begin
  # All playlists.
  data, status_code, headers = api_instance.all_playlists_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<PlaylistLargeDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->all_playlists_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **include_recordings** | **Boolean** | Whether a playlist shall include recordings or not. | [optional][default to false] |
| **ignore_usages** | **Boolean** | Whether a playlist shall include all songs regardless of their track usages. | [optional][default to false] |
| **usage_filter_mode** | **String** | Whether a playlist recordings shall include all playlist usages or not. | [optional][default to &#39;any&#39;] |
| **songtradr_playlist_guid** | **String** |  | [optional] |

### Return type

[**Array&lt;PlaylistLargeDTO&gt;**](PlaylistLargeDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## create_or_update_playlist

> Object create_or_update_playlist(save_playlist_dto)

Create and edit playlist.

This endpoint expects always the full amount of information including all recordings.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::PlaylistApi.new
save_playlist_dto = SongtradrApiClientRuby::SavePlaylistDTO.new({songtradr_playlist_guid: 'songtradr_playlist_guid_example', name: 'name_example', state: 'active', usages: ['usages_example']}) # SavePlaylistDTO | 

begin
  # Create and edit playlist.
  result = api_instance.create_or_update_playlist(save_playlist_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->create_or_update_playlist: #{e}"
end
```

#### Using the create_or_update_playlist_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> create_or_update_playlist_with_http_info(save_playlist_dto)

```ruby
begin
  # Create and edit playlist.
  data, status_code, headers = api_instance.create_or_update_playlist_with_http_info(save_playlist_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->create_or_update_playlist_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **save_playlist_dto** | [**SavePlaylistDTO**](SavePlaylistDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## curate_playlist

> <CuratePlaylistResponseDTO> curate_playlist(method_name, curate_playlist_dto)

Curate playlist.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::PlaylistApi.new
method_name = 'recommend' # String | Name of the curation task that should be executed
curate_playlist_dto = SongtradrApiClientRuby::CuratePlaylistDTO.new # CuratePlaylistDTO | 

begin
  # Curate playlist.
  result = api_instance.curate_playlist(method_name, curate_playlist_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->curate_playlist: #{e}"
end
```

#### Using the curate_playlist_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CuratePlaylistResponseDTO>, Integer, Hash)> curate_playlist_with_http_info(method_name, curate_playlist_dto)

```ruby
begin
  # Curate playlist.
  data, status_code, headers = api_instance.curate_playlist_with_http_info(method_name, curate_playlist_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CuratePlaylistResponseDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->curate_playlist_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **method_name** | **String** | Name of the curation task that should be executed |  |
| **curate_playlist_dto** | [**CuratePlaylistDTO**](CuratePlaylistDTO.md) |  |  |

### Return type

[**CuratePlaylistResponseDTO**](CuratePlaylistResponseDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_playlist

> Object delete_playlist(songtradr_playlist_guid)

Delete playlist.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::PlaylistApi.new
songtradr_playlist_guid = '1234' # String | ID of the file that should be deleted.

begin
  # Delete playlist.
  result = api_instance.delete_playlist(songtradr_playlist_guid)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->delete_playlist: #{e}"
end
```

#### Using the delete_playlist_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_playlist_with_http_info(songtradr_playlist_guid)

```ruby
begin
  # Delete playlist.
  data, status_code, headers = api_instance.delete_playlist_with_http_info(songtradr_playlist_guid)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PlaylistApi->delete_playlist_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **songtradr_playlist_guid** | **String** | ID of the file that should be deleted. |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/hal+json, application/json

