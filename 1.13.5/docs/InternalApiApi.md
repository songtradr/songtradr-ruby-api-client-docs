# SongtradrApiClientRuby::InternalApiApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**internal_create_inference**](InternalApiApi.md#internal_create_inference) | **POST** /api/v1/internal/inference |  |
| [**internal_update_file**](InternalApiApi.md#internal_update_file) | **PATCH** /api/v1/internal/file/{customerName}/{objectKey} |  |


## internal_create_inference

> Object internal_create_inference(authorization, save_file_recording_dto)



### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::InternalApiApi.new
authorization = 'authorization_example' # String | 
save_file_recording_dto = [SongtradrApiClientRuby::SaveFileRecordingDTO.new({isrc: 'isrc_example', created_by_version: 'created_by_version_example'})] # Array<SaveFileRecordingDTO> | 

begin
  
  result = api_instance.internal_create_inference(authorization, save_file_recording_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling InternalApiApi->internal_create_inference: #{e}"
end
```

#### Using the internal_create_inference_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> internal_create_inference_with_http_info(authorization, save_file_recording_dto)

```ruby
begin
  
  data, status_code, headers = api_instance.internal_create_inference_with_http_info(authorization, save_file_recording_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling InternalApiApi->internal_create_inference_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **authorization** | **String** |  |  |
| **save_file_recording_dto** | [**Array&lt;SaveFileRecordingDTO&gt;**](SaveFileRecordingDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## internal_update_file

> Object internal_update_file(customer_name, object_key, save_file_dto)



### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::InternalApiApi.new
customer_name = 'customer_name_example' # String | 
object_key = 'object_key_example' # String | 
save_file_dto = SongtradrApiClientRuby::SaveFileDTO.new # SaveFileDTO | 

begin
  
  result = api_instance.internal_update_file(customer_name, object_key, save_file_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling InternalApiApi->internal_update_file: #{e}"
end
```

#### Using the internal_update_file_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> internal_update_file_with_http_info(customer_name, object_key, save_file_dto)

```ruby
begin
  
  data, status_code, headers = api_instance.internal_update_file_with_http_info(customer_name, object_key, save_file_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling InternalApiApi->internal_update_file_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **customer_name** | **String** |  |  |
| **object_key** | **String** |  |  |
| **save_file_dto** | [**SaveFileDTO**](SaveFileDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

