# SongtradrApiClientRuby::AdminUsersControllerApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_user**](AdminUsersControllerApi.md#create_user) | **POST** /api/v1/admin/users | create a user |
| [**delete_user**](AdminUsersControllerApi.md#delete_user) | **DELETE** /api/v1/admin/users/{id} | delete a user |
| [**get_user**](AdminUsersControllerApi.md#get_user) | **GET** /api/v1/admin/users/{id} | show details of a user |
| [**get_users**](AdminUsersControllerApi.md#get_users) | **GET** /api/v1/admin/users | List users |
| [**update_user**](AdminUsersControllerApi.md#update_user) | **PUT** /api/v1/admin/users/{id} | update a user |


## create_user

> <AdminApiUserDTO> create_user(admin_api_create_user_dto)

create a user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::AdminUsersControllerApi.new
admin_api_create_user_dto = SongtradrApiClientRuby::AdminApiCreateUserDTO.new({email: 'email_example', full_name: 'full_name_example'}) # AdminApiCreateUserDTO | 

begin
  # create a user
  result = api_instance.create_user(admin_api_create_user_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->create_user: #{e}"
end
```

#### Using the create_user_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AdminApiUserDTO>, Integer, Hash)> create_user_with_http_info(admin_api_create_user_dto)

```ruby
begin
  # create a user
  data, status_code, headers = api_instance.create_user_with_http_info(admin_api_create_user_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AdminApiUserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->create_user_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **admin_api_create_user_dto** | [**AdminApiCreateUserDTO**](AdminApiCreateUserDTO.md) |  |  |

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_user

> Object delete_user(id)

delete a user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::AdminUsersControllerApi.new
id = 56 # Integer | 

begin
  # delete a user
  result = api_instance.delete_user(id)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->delete_user: #{e}"
end
```

#### Using the delete_user_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_user_with_http_info(id)

```ruby
begin
  # delete a user
  data, status_code, headers = api_instance.delete_user_with_http_info(id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->delete_user_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Integer** |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_user

> <AdminApiUserDTO> get_user(id)

show details of a user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::AdminUsersControllerApi.new
id = 56 # Integer | 

begin
  # show details of a user
  result = api_instance.get_user(id)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->get_user: #{e}"
end
```

#### Using the get_user_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AdminApiUserDTO>, Integer, Hash)> get_user_with_http_info(id)

```ruby
begin
  # show details of a user
  data, status_code, headers = api_instance.get_user_with_http_info(id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AdminApiUserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->get_user_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Integer** |  |  |

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_users

> <AdminApiUserDTO> get_users(opts)

List users

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::AdminUsersControllerApi.new
opts = {
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # List users
  result = api_instance.get_users(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->get_users: #{e}"
end
```

#### Using the get_users_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AdminApiUserDTO>, Integer, Hash)> get_users_with_http_info(opts)

```ruby
begin
  # List users
  data, status_code, headers = api_instance.get_users_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AdminApiUserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->get_users_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_user

> <AdminApiUserDTO> update_user(id, admin_api_update_user_dto)

update a user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::AdminUsersControllerApi.new
id = 56 # Integer | 
admin_api_update_user_dto = SongtradrApiClientRuby::AdminApiUpdateUserDTO.new # AdminApiUpdateUserDTO | 

begin
  # update a user
  result = api_instance.update_user(id, admin_api_update_user_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->update_user: #{e}"
end
```

#### Using the update_user_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<AdminApiUserDTO>, Integer, Hash)> update_user_with_http_info(id, admin_api_update_user_dto)

```ruby
begin
  # update a user
  data, status_code, headers = api_instance.update_user_with_http_info(id, admin_api_update_user_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <AdminApiUserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling AdminUsersControllerApi->update_user_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Integer** |  |  |
| **admin_api_update_user_dto** | [**AdminApiUpdateUserDTO**](AdminApiUpdateUserDTO.md) |  |  |

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

