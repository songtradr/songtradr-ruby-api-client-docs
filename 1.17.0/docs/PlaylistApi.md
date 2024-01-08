# SongtradrApiClientRuby::PlaylistApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**curate_playlist**](PlaylistApi.md#curate_playlist) | **POST** /api/v1/playlist/{methodName} | Curate playlist. |


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

