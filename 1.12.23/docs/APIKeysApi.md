# SongtradrApiClientRuby::APIKeysApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_api_key**](APIKeysApi.md#create_api_key) | **POST** /api/v1/user/apiKeys | create an API key |
| [**delete_api_key**](APIKeysApi.md#delete_api_key) | **DELETE** /api/v1/user/apiKeys/{id} | delete an API key |
| [**get_api_keys**](APIKeysApi.md#get_api_keys) | **GET** /api/v1/user/apiKeys | list API keys |


## create_api_key

> <AdminApiUserDTO> create_api_key(create_api_key_dto)

create an API key

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::APIKeysApi.new
create_api_key_dto = SongtradrApiClientRuby::CreateApiKeyDTO.new # CreateApiKeyDTO | 

begin
  # create an API key
  result = api_instance.create_api_key(create_api_key_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key: #{e}"
end
```

#### Using the create_api_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AdminApiUserDTO>, Integer, Hash)> create_api_key_with_http_info(create_api_key_dto)

```ruby
begin
  # create an API key
  data, status_code, headers = api_instance.create_api_key_with_http_info(create_api_key_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AdminApiUserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **create_api_key_dto** | [**CreateApiKeyDTO**](CreateApiKeyDTO.md) |  |  |

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_api_key

> Object delete_api_key(id)

delete an API key

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::APIKeysApi.new
id = 'id_example' # String | 

begin
  # delete an API key
  result = api_instance.delete_api_key(id)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->delete_api_key: #{e}"
end
```

#### Using the delete_api_key_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_api_key_with_http_info(id)

```ruby
begin
  # delete an API key
  data, status_code, headers = api_instance.delete_api_key_with_http_info(id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->delete_api_key_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_api_keys

> <Array<ApiKeyDTO>> get_api_keys(opts)

list API keys

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::APIKeysApi.new
opts = {
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # list API keys
  result = api_instance.get_api_keys(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->get_api_keys: #{e}"
end
```

#### Using the get_api_keys_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<ApiKeyDTO>>, Integer, Hash)> get_api_keys_with_http_info(opts)

```ruby
begin
  # list API keys
  data, status_code, headers = api_instance.get_api_keys_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<ApiKeyDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling APIKeysApi->get_api_keys_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**Array&lt;ApiKeyDTO&gt;**](ApiKeyDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

