# SongtradrApiClientRuby::AllowedValuesApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**allowed_musical_features**](AllowedValuesApi.md#allowed_musical_features) | **GET** /api/v1/allowedValues/musicalFeatures | Allowed values for music descriptive parameters to be used in the searchAll endpoint. |
| [**genres**](AllowedValuesApi.md#genres) | **GET** /api/v1/allowedValues/genre | Allowed values for genres. |
| [**tags**](AllowedValuesApi.md#tags) | **GET** /api/v1/allowedValues/tag | All descriptive tags inside of tag-categories. |


## allowed_musical_features

> <SearchFilterValuesDTO> allowed_musical_features(opts)

Allowed values for music descriptive parameters to be used in the searchAll endpoint.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'

api_instance = SongtradrApiClientRuby::AllowedValuesApi.new
opts = {
  response_size: 's' # String | Size the response should have.
}

begin
  # Allowed values for music descriptive parameters to be used in the searchAll endpoint.
  result = api_instance.allowed_musical_features(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->allowed_musical_features: #{e}"
end
```

#### Using the allowed_musical_features_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SearchFilterValuesDTO>, Integer, Hash)> allowed_musical_features_with_http_info(opts)

```ruby
begin
  # Allowed values for music descriptive parameters to be used in the searchAll endpoint.
  data, status_code, headers = api_instance.allowed_musical_features_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SearchFilterValuesDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->allowed_musical_features_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **response_size** | **String** | Size the response should have. | [optional][default to &#39;s&#39;] |

### Return type

[**SearchFilterValuesDTO**](SearchFilterValuesDTO.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## genres

> <Array<GenreDTO>> genres(genre_type)

Allowed values for genres.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'

api_instance = SongtradrApiClientRuby::AllowedValuesApi.new
genre_type = 'level1Genre' # String | Type of the response should have.

begin
  # Allowed values for genres.
  result = api_instance.genres(genre_type)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->genres: #{e}"
end
```

#### Using the genres_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<GenreDTO>>, Integer, Hash)> genres_with_http_info(genre_type)

```ruby
begin
  # Allowed values for genres.
  data, status_code, headers = api_instance.genres_with_http_info(genre_type)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<GenreDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->genres_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **genre_type** | **String** | Type of the response should have. |  |

### Return type

[**Array&lt;GenreDTO&gt;**](GenreDTO.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## tags

> <Array<CategoryMediumDTO>> tags(opts)

All descriptive tags inside of tag-categories.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'

api_instance = SongtradrApiClientRuby::AllowedValuesApi.new
opts = {
  category_name: 'mood' # String | Filters tags for one category only 
}

begin
  # All descriptive tags inside of tag-categories.
  result = api_instance.tags(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->tags: #{e}"
end
```

#### Using the tags_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<CategoryMediumDTO>>, Integer, Hash)> tags_with_http_info(opts)

```ruby
begin
  # All descriptive tags inside of tag-categories.
  data, status_code, headers = api_instance.tags_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<CategoryMediumDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AllowedValuesApi->tags_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **category_name** | **String** | Filters tags for one category only  | [optional] |

### Return type

[**Array&lt;CategoryMediumDTO&gt;**](CategoryMediumDTO.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

