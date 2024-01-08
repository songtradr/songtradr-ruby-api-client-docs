# SongtradrApiClientRuby::RecordingApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**recordings_by_ids_with_musical_features**](RecordingApi.md#recordings_by_ids_with_musical_features) | **GET** /api/v1/public/recording/{ids}/musicalFeatures | AI generated moods, musical features and more for recordings. |
| [**recordings_by_ids_with_similarities**](RecordingApi.md#recordings_by_ids_with_similarities) | **GET** /api/v1/public/recording/{ids}/similarities | Similar recordings for a list of recordings. |
| [**recordings_by_ids_with_taggrams**](RecordingApi.md#recordings_by_ids_with_taggrams) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings. |
| [**recordings_by_ids_with_tagstrengths**](RecordingApi.md#recordings_by_ids_with_tagstrengths) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings. |
| [**recordings_medium_by_ids**](RecordingApi.md#recordings_medium_by_ids) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response. |
| [**search_recordings**](RecordingApi.md#search_recordings) | **GET** /api/v1/public/recording/search | Recordings by contributors, moods, musical features and more. |
| [**search_recordings_granular**](RecordingApi.md#search_recordings_granular) | **POST** /api/v1/public/recording/searchGranular | Recordings by granular search options. |


## recordings_by_ids_with_musical_features

> <Array<RecordingMinimalWithMusicalFeaturesDTO>> recordings_by_ids_with_musical_features(ids)

AI generated moods, musical features and more for recordings.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
ids = 'ZAA010800469' # String | Comma seperated list of IDs. Can be ISRCs or proprietary IDs

begin
  # AI generated moods, musical features and more for recordings.
  result = api_instance.recordings_by_ids_with_musical_features(ids)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_musical_features: #{e}"
end
```

#### Using the recordings_by_ids_with_musical_features_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMinimalWithMusicalFeaturesDTO>>, Integer, Hash)> recordings_by_ids_with_musical_features_with_http_info(ids)

```ruby
begin
  # AI generated moods, musical features and more for recordings.
  data, status_code, headers = api_instance.recordings_by_ids_with_musical_features_with_http_info(ids)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMinimalWithMusicalFeaturesDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_musical_features_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ids** | **String** | Comma seperated list of IDs. Can be ISRCs or proprietary IDs |  |

### Return type

[**Array&lt;RecordingMinimalWithMusicalFeaturesDTO&gt;**](RecordingMinimalWithMusicalFeaturesDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_by_ids_with_similarities

> <Array<RecordingForSimilaritySearchDTO>> recordings_by_ids_with_similarities(ids, opts)

Similar recordings for a list of recordings.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
ids = 'USUM71703692' # String | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
opts = {
  identical_only: true, # Boolean | Whether a result list shall include only identical recordings.
  usage: 'usage_example' # String | Filter by recording usage.
}

begin
  # Similar recordings for a list of recordings.
  result = api_instance.recordings_by_ids_with_similarities(ids, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_similarities: #{e}"
end
```

#### Using the recordings_by_ids_with_similarities_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingForSimilaritySearchDTO>>, Integer, Hash)> recordings_by_ids_with_similarities_with_http_info(ids, opts)

```ruby
begin
  # Similar recordings for a list of recordings.
  data, status_code, headers = api_instance.recordings_by_ids_with_similarities_with_http_info(ids, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingForSimilaritySearchDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_similarities_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ids** | **String** | Comma seperated list of IDs. Can be ISRCs or proprietary IDs |  |
| **identical_only** | **Boolean** | Whether a result list shall include only identical recordings. | [optional][default to false] |
| **usage** | **String** | Filter by recording usage. | [optional] |

### Return type

[**Array&lt;RecordingForSimilaritySearchDTO&gt;**](RecordingForSimilaritySearchDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_by_ids_with_taggrams

> <Array<RecordingMinimalWithTaggramsDTO>> recordings_by_ids_with_taggrams(ids, opts)

Timeseries of AI generated moods, musical features and more for a list of recordings.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
ids = 'USUM71703692' # String | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
opts = {
  category_name: 'instrument', # String | Show only taggrams for one category.
  tag_name: 'energetic', # String | Show only taggrams for one tag.
  genre_name: 'Ska', # String | Show only taggrams for one genre.
  from_timestamp: 16.0, # Float | Show only taggrams data starting from from this timestamp in seconds.
  to_timestamp: 32.0, # Float | Show only taggrams data before this timestamp in seconds.
  fill_with_zero: true # Boolean | If set to true, empty timeseries are filled with timeseries of 0.0 values.
}

begin
  # Timeseries of AI generated moods, musical features and more for a list of recordings.
  result = api_instance.recordings_by_ids_with_taggrams(ids, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_taggrams: #{e}"
end
```

#### Using the recordings_by_ids_with_taggrams_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMinimalWithTaggramsDTO>>, Integer, Hash)> recordings_by_ids_with_taggrams_with_http_info(ids, opts)

```ruby
begin
  # Timeseries of AI generated moods, musical features and more for a list of recordings.
  data, status_code, headers = api_instance.recordings_by_ids_with_taggrams_with_http_info(ids, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMinimalWithTaggramsDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_taggrams_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ids** | **String** | Comma seperated list of IDs. Can be ISRCs or proprietary IDs |  |
| **category_name** | **String** | Show only taggrams for one category. | [optional] |
| **tag_name** | **String** | Show only taggrams for one tag. | [optional] |
| **genre_name** | **String** | Show only taggrams for one genre. | [optional] |
| **from_timestamp** | **Float** | Show only taggrams data starting from from this timestamp in seconds. | [optional] |
| **to_timestamp** | **Float** | Show only taggrams data before this timestamp in seconds. | [optional] |
| **fill_with_zero** | **Boolean** | If set to true, empty timeseries are filled with timeseries of 0.0 values. | [optional] |

### Return type

[**Array&lt;RecordingMinimalWithTaggramsDTO&gt;**](RecordingMinimalWithTaggramsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_by_ids_with_tagstrengths

> <Array<RecordingMinimalWithTagstrengthsDTO>> recordings_by_ids_with_tagstrengths(ids, opts)

Strengths as numerical representations for AI generated moods, musical features and more for recordings.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
ids = 'USUM71703692' # String | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
opts = {
  category_name: 'instrument', # String | Show only taggrams for one category.
  tag_name: 'energetic', # String | Show only taggrams for one tag.
  genre_name: 'Ska' # String | Show only taggrams for one genre.
}

begin
  # Strengths as numerical representations for AI generated moods, musical features and more for recordings.
  result = api_instance.recordings_by_ids_with_tagstrengths(ids, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_tagstrengths: #{e}"
end
```

#### Using the recordings_by_ids_with_tagstrengths_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMinimalWithTagstrengthsDTO>>, Integer, Hash)> recordings_by_ids_with_tagstrengths_with_http_info(ids, opts)

```ruby
begin
  # Strengths as numerical representations for AI generated moods, musical features and more for recordings.
  data, status_code, headers = api_instance.recordings_by_ids_with_tagstrengths_with_http_info(ids, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMinimalWithTagstrengthsDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_by_ids_with_tagstrengths_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ids** | **String** | Comma seperated list of IDs. Can be ISRCs or proprietary IDs |  |
| **category_name** | **String** | Show only taggrams for one category. | [optional] |
| **tag_name** | **String** | Show only taggrams for one tag. | [optional] |
| **genre_name** | **String** | Show only taggrams for one genre. | [optional] |

### Return type

[**Array&lt;RecordingMinimalWithTagstrengthsDTO&gt;**](RecordingMinimalWithTagstrengthsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_medium_by_ids

> <Array<RecordingMediumDTO>> recordings_medium_by_ids(ids, opts)

Recordings by IDs with a medium sized response.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
ids = 'GBAHT0108619' # String | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
opts = {
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # Recordings by IDs with a medium sized response.
  result = api_instance.recordings_medium_by_ids(ids, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_medium_by_ids: #{e}"
end
```

#### Using the recordings_medium_by_ids_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMediumDTO>>, Integer, Hash)> recordings_medium_by_ids_with_http_info(ids, opts)

```ruby
begin
  # Recordings by IDs with a medium sized response.
  data, status_code, headers = api_instance.recordings_medium_by_ids_with_http_info(ids, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMediumDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->recordings_medium_by_ids_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **ids** | **String** | Comma seperated list of IDs. Can be ISRCs or proprietary IDs |  |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**Array&lt;RecordingMediumDTO&gt;**](RecordingMediumDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## search_recordings

> <RecordingListDTO> search_recordings(opts)

Recordings by contributors, moods, musical features and more.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
opts = {
  similar_to_recording: 'GBUM71110209', # String | Search for songs similar to a recording.
  contributor: 'Rick Rubin', # String | Search for a name that was involved as any contributor.
  main_artist: 'The Beatles', # String | Search for a main artist.
  composer: 'John Cale', # String | Search for a composer.
  title: 'Highway To Hell', # String | Search for a title.
  party_and_title: 'The Beatles yesterday', # String | Search for party and title.
  language: 'en', # String | Search for a language of the lyrics.
  genre: 'Rock', # String | Search for a genre.
  primary_mood_cluster: 'aggressive', # String | Search for a mood.
  valence: 'very sad', # String | Search for valence.
  arousal: 'very calm', # String | Search for arousal.
  pleasantness: 'very unpleasant', # String | Search for pleasantness.
  engagement: 'very unengaging', # String | Search for an engagement.
  vocals: 'instrumental', # String | Search for a vocals gender or instrumental songs.
  dominant_instrument: 'electric guitar', # String | Search for a dominant instrument.
  energy: 'very quiet', # String | Search for energy.
  sound_generation: 'acoustic', # String | Search for type of sound generation.
  tempo: 'very slow', # String | Search for tempo.
  scale: 'major key', # String | Search for tonal scale.
  key: 'C', # String | Search for harmonic key.
  rhythm: 'common time', # String | Search for rhythm.
  primary_sound_character: 'brassy', # String | Search for a sound character.
  timbre: 'very warm', # String | Search for timbre.
  roughness: 'very clear', # String | Search for roughness.
  tonality: 'monotonous', # String | Search for tonality.
  harmony: 'very dissonant', # String | Search for a degree of harmoniousness.
  texture: 'very thin', # String | Search for texture.
  groovyness: 'very steady', # String | Search for groovyness.
  space: 'very compact', # String | Search for space.
  origin_decade: 'pre-1950s', # String | Search for origin decade.
  curateability: 'curateable', # String | Search for curateability.
  use_case: 'background', # String | Search for use case.
  channel_suitability: 'Spotify', # String | Search for channel suitability.
  songtradr_track_id: 'songtradr_track_id_example', # String | Search for Songtradr track id.
  usage: 'usage_example', # String | Search for recording usage.
  similar_to_songtradr_track_id: '1bF118m', # String | Search for songs similar to a recording by songtradr Track Id.
  shuffled: 'true', # String | Sort the results randomly.
  sort: 'popularityDesc', # String | Sort the results.
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56 # Integer | The size of the page to be returned
}

begin
  # Recordings by contributors, moods, musical features and more.
  result = api_instance.search_recordings(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->search_recordings: #{e}"
end
```

#### Using the search_recordings_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RecordingListDTO>, Integer, Hash)> search_recordings_with_http_info(opts)

```ruby
begin
  # Recordings by contributors, moods, musical features and more.
  data, status_code, headers = api_instance.search_recordings_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RecordingListDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->search_recordings_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **similar_to_recording** | **String** | Search for songs similar to a recording. | [optional] |
| **contributor** | **String** | Search for a name that was involved as any contributor. | [optional] |
| **main_artist** | **String** | Search for a main artist. | [optional] |
| **composer** | **String** | Search for a composer. | [optional] |
| **title** | **String** | Search for a title. | [optional] |
| **party_and_title** | **String** | Search for party and title. | [optional] |
| **language** | **String** | Search for a language of the lyrics. | [optional] |
| **genre** | **String** | Search for a genre. | [optional] |
| **primary_mood_cluster** | **String** | Search for a mood. | [optional] |
| **valence** | **String** | Search for valence. | [optional] |
| **arousal** | **String** | Search for arousal. | [optional] |
| **pleasantness** | **String** | Search for pleasantness. | [optional] |
| **engagement** | **String** | Search for an engagement. | [optional] |
| **vocals** | **String** | Search for a vocals gender or instrumental songs. | [optional] |
| **dominant_instrument** | **String** | Search for a dominant instrument. | [optional] |
| **energy** | **String** | Search for energy. | [optional] |
| **sound_generation** | **String** | Search for type of sound generation. | [optional] |
| **tempo** | **String** | Search for tempo. | [optional] |
| **scale** | **String** | Search for tonal scale. | [optional] |
| **key** | **String** | Search for harmonic key. | [optional] |
| **rhythm** | **String** | Search for rhythm. | [optional] |
| **primary_sound_character** | **String** | Search for a sound character. | [optional] |
| **timbre** | **String** | Search for timbre. | [optional] |
| **roughness** | **String** | Search for roughness. | [optional] |
| **tonality** | **String** | Search for tonality. | [optional] |
| **harmony** | **String** | Search for a degree of harmoniousness. | [optional] |
| **texture** | **String** | Search for texture. | [optional] |
| **groovyness** | **String** | Search for groovyness. | [optional] |
| **space** | **String** | Search for space. | [optional] |
| **origin_decade** | **String** | Search for origin decade. | [optional] |
| **curateability** | **String** | Search for curateability. | [optional] |
| **use_case** | **String** | Search for use case. | [optional] |
| **channel_suitability** | **String** | Search for channel suitability. | [optional] |
| **songtradr_track_id** | **String** | Search for Songtradr track id. | [optional] |
| **usage** | **String** | Search for recording usage. | [optional] |
| **similar_to_songtradr_track_id** | **String** | Search for songs similar to a recording by songtradr Track Id. | [optional] |
| **shuffled** | **String** | Sort the results randomly. | [optional][default to &#39;false&#39;] |
| **sort** | **String** | Sort the results. | [optional][default to &#39;popularityDesc&#39;] |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |

### Return type

[**RecordingListDTO**](RecordingListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## search_recordings_granular

> <RecordingListDTO> search_recordings_granular(search_recording_granular_dto)

Recordings by granular search options.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::RecordingApi.new
search_recording_granular_dto = [SongtradrApiClientRuby::SearchRecordingGranularDTO.new({tag_name: 'tag_name_example'})] # Array<SearchRecordingGranularDTO> | 

begin
  # Recordings by granular search options.
  result = api_instance.search_recordings_granular(search_recording_granular_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->search_recordings_granular: #{e}"
end
```

#### Using the search_recordings_granular_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<RecordingListDTO>, Integer, Hash)> search_recordings_granular_with_http_info(search_recording_granular_dto)

```ruby
begin
  # Recordings by granular search options.
  data, status_code, headers = api_instance.search_recordings_granular_with_http_info(search_recording_granular_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <RecordingListDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling RecordingApi->search_recordings_granular_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **search_recording_granular_dto** | [**Array&lt;SearchRecordingGranularDTO&gt;**](SearchRecordingGranularDTO.md) |  |  |

### Return type

[**RecordingListDTO**](RecordingListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

