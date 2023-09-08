# SongtradrApiClientRuby::PartyApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**party**](PartyApi.md#party) | **GET** /api/v1/party | Information on a person, group or company. |


## party

> <PartyLargeDTO> party(full_name)

Information on a person, group or company.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::PartyApi.new
full_name = 'The Beatles' # String | Full Name of the person, group, company or organisation.

begin
  # Information on a person, group or company.
  result = api_instance.party(full_name)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PartyApi->party: #{e}"
end
```

#### Using the party_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PartyLargeDTO>, Integer, Hash)> party_with_http_info(full_name)

```ruby
begin
  # Information on a person, group or company.
  data, status_code, headers = api_instance.party_with_http_info(full_name)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PartyLargeDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling PartyApi->party_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **full_name** | **String** | Full Name of the person, group, company or organisation. |  |

### Return type

[**PartyLargeDTO**](PartyLargeDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

