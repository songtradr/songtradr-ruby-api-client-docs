# SongtradrApiClientRuby::UserApi

All URIs are relative to *https://api.songtradr.com*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**delete_user_file**](UserApi.md#delete_user_file) | **DELETE** /api/v1/user/file/{objectKey} | Delete file. |
| [**edit_me**](UserApi.md#edit_me) | **POST** /api/v1/user/me | Edit details for a logged-in user |
| [**forgot_password**](UserApi.md#forgot_password) | **POST** /api/v1/user/forgot-password | Send a password reset email |
| [**init_video_upload**](UserApi.md#init_video_upload) | **POST** /api/v1/user/file/{name}/initVideoUpload | Recognise and upload video. Responds with an object with recognition result. |
| [**initiate_user_file_upload**](UserApi.md#initiate_user_file_upload) | **POST** /api/v1/user/file/{name}/initUpload | Initialize a file upload. Responds with an URL where the file can be uploaded. |
| [**initiate_user_image_upload**](UserApi.md#initiate_user_image_upload) | **POST** /api/v1/user/file/{name}/initImageUpload | Recognise and upload image. Responds with an object with recognition result. |
| [**login**](UserApi.md#login) | **POST** /api/v1/user/login | Login to generate a bearer token. |
| [**me**](UserApi.md#me) | **GET** /api/v1/user/me | Details for a logged-in user |
| [**prompt_search_user_files**](UserApi.md#prompt_search_user_files) | **GET** /api/v1/user/promptSearch | Files for query. |
| [**recordings_by_folder_with_taggrams**](UserApi.md#recordings_by_folder_with_taggrams) | **GET** /api/v1/user/folder/{folderName}/taggrams | Timeseries of AI generated moods, musical features and more for recordings in your folder. |
| [**recordings_by_folder_with_tagstrengths**](UserApi.md#recordings_by_folder_with_tagstrengths) | **GET** /api/v1/user/folder/{folderName}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder. |
| [**sign_up**](UserApi.md#sign_up) | **POST** /api/v1/user/sign-up | Sign up a new user. |
| [**token**](UserApi.md#token) | **POST** /api/v1/user/token | Generates a new JWT token for the given refresh token |
| [**update_password**](UserApi.md#update_password) | **POST** /api/v1/user/update-password | Update password by using the password reset token |
| [**user_file**](UserApi.md#user_file) | **GET** /api/v1/user/file/{objectKey} | Details and a download link for a file. |
| [**user_files**](UserApi.md#user_files) | **GET** /api/v1/user/files | List and search your own files. |
| [**user_files_status**](UserApi.md#user_files_status) | **GET** /api/v1/user/filesStatus | Status details for files. |
| [**user_files_summary**](UserApi.md#user_files_summary) | **GET** /api/v1/user/filesSummary | Summary fo your files. |


## delete_user_file

> Object delete_user_file(object_key)

Delete file.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
object_key = '73818371-0963-412e-aa3d-27c2bab952a3' # String | ObjectKey of the file that should be deleted.

begin
  # Delete file.
  result = api_instance.delete_user_file(object_key)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->delete_user_file: #{e}"
end
```

#### Using the delete_user_file_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_user_file_with_http_info(object_key)

```ruby
begin
  # Delete file.
  data, status_code, headers = api_instance.delete_user_file_with_http_info(object_key)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->delete_user_file_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **object_key** | **String** | ObjectKey of the file that should be deleted. |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/hal+json, application/json


## edit_me

> Object edit_me(save_user_dto)

Edit details for a logged-in user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
save_user_dto = SongtradrApiClientRuby::SaveUserDTO.new({email_address: 'email_address_example'}) # SaveUserDTO | 

begin
  # Edit details for a logged-in user
  result = api_instance.edit_me(save_user_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->edit_me: #{e}"
end
```

#### Using the edit_me_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> edit_me_with_http_info(save_user_dto)

```ruby
begin
  # Edit details for a logged-in user
  data, status_code, headers = api_instance.edit_me_with_http_info(save_user_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->edit_me_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **save_user_dto** | [**SaveUserDTO**](SaveUserDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## forgot_password

> Object forgot_password(forgot_password_dto)

Send a password reset email

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
forgot_password_dto = SongtradrApiClientRuby::ForgotPasswordDTO.new({email_or_username: 'email_or_username_example'}) # ForgotPasswordDTO | 

begin
  # Send a password reset email
  result = api_instance.forgot_password(forgot_password_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->forgot_password: #{e}"
end
```

#### Using the forgot_password_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> forgot_password_with_http_info(forgot_password_dto)

```ruby
begin
  # Send a password reset email
  data, status_code, headers = api_instance.forgot_password_with_http_info(forgot_password_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->forgot_password_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **forgot_password_dto** | [**ForgotPasswordDTO**](ForgotPasswordDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/hal+json, application/json


## init_video_upload

> <VideoRecognitionResponse> init_video_upload(name, url)

Recognise and upload video. Responds with an object with recognition result.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
name = 'FileName.mp4' # String | The Name of the image that will be uploaded
url = 'url_example' # String | 

begin
  # Recognise and upload video. Responds with an object with recognition result.
  result = api_instance.init_video_upload(name, url)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->init_video_upload: #{e}"
end
```

#### Using the init_video_upload_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<VideoRecognitionResponse>, Integer, Hash)> init_video_upload_with_http_info(name, url)

```ruby
begin
  # Recognise and upload video. Responds with an object with recognition result.
  data, status_code, headers = api_instance.init_video_upload_with_http_info(name, url)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <VideoRecognitionResponse>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->init_video_upload_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** | The Name of the image that will be uploaded |  |
| **url** | **String** |  |  |

### Return type

[**VideoRecognitionResponse**](VideoRecognitionResponse.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## initiate_user_file_upload

> <InitPutRecordingAudioDTO> initiate_user_file_upload(name, folder, opts)

Initialize a file upload. Responds with an URL where the file can be uploaded.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
name = 'FileName.mp3' # String | The Name of the file that will be uploaded
folder = 'FolderName' # String | The Name of the folder that the file will be placed in
opts = {
  file_upload_dto: SongtradrApiClientRuby::FileUploadDTO.new # FileUploadDTO | 
}

begin
  # Initialize a file upload. Responds with an URL where the file can be uploaded.
  result = api_instance.initiate_user_file_upload(name, folder, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->initiate_user_file_upload: #{e}"
end
```

#### Using the initiate_user_file_upload_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<InitPutRecordingAudioDTO>, Integer, Hash)> initiate_user_file_upload_with_http_info(name, folder, opts)

```ruby
begin
  # Initialize a file upload. Responds with an URL where the file can be uploaded.
  data, status_code, headers = api_instance.initiate_user_file_upload_with_http_info(name, folder, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <InitPutRecordingAudioDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->initiate_user_file_upload_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** | The Name of the file that will be uploaded |  |
| **folder** | **String** | The Name of the folder that the file will be placed in |  |
| **file_upload_dto** | [**FileUploadDTO**](FileUploadDTO.md) |  | [optional] |

### Return type

[**InitPutRecordingAudioDTO**](InitPutRecordingAudioDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## initiate_user_image_upload

> <ImageRecognitionResponse> initiate_user_image_upload(name, url)

Recognise and upload image. Responds with an object with recognition result.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
name = 'FileName.mp3' # String | The Name of the image that will be uploaded
url = 'url_example' # String | 

begin
  # Recognise and upload image. Responds with an object with recognition result.
  result = api_instance.initiate_user_image_upload(name, url)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->initiate_user_image_upload: #{e}"
end
```

#### Using the initiate_user_image_upload_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ImageRecognitionResponse>, Integer, Hash)> initiate_user_image_upload_with_http_info(name, url)

```ruby
begin
  # Recognise and upload image. Responds with an object with recognition result.
  data, status_code, headers = api_instance.initiate_user_image_upload_with_http_info(name, url)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ImageRecognitionResponse>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->initiate_user_image_upload_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** | The Name of the image that will be uploaded |  |
| **url** | **String** |  |  |

### Return type

[**ImageRecognitionResponse**](ImageRecognitionResponse.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## login

> <JwtTokenDTO> login(login_dto)

Login to generate a bearer token.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
login_dto = SongtradrApiClientRuby::LoginDTO.new({email: 'email_example', password: 'password_example'}) # LoginDTO | 

begin
  # Login to generate a bearer token.
  result = api_instance.login(login_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->login: #{e}"
end
```

#### Using the login_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JwtTokenDTO>, Integer, Hash)> login_with_http_info(login_dto)

```ruby
begin
  # Login to generate a bearer token.
  data, status_code, headers = api_instance.login_with_http_info(login_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JwtTokenDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->login_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **login_dto** | [**LoginDTO**](LoginDTO.md) |  |  |

### Return type

[**JwtTokenDTO**](JwtTokenDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## me

> <UserDTO> me

Details for a logged-in user

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new

begin
  # Details for a logged-in user
  result = api_instance.me
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->me: #{e}"
end
```

#### Using the me_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<UserDTO>, Integer, Hash)> me_with_http_info

```ruby
begin
  # Details for a logged-in user
  data, status_code, headers = api_instance.me_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <UserDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->me_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserDTO**](UserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## prompt_search_user_files

> <FileListDTO> prompt_search_user_files(query)

Files for query.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
query = 'funk, guitar, drums' # String | Query.

begin
  # Files for query.
  result = api_instance.prompt_search_user_files(query)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->prompt_search_user_files: #{e}"
end
```

#### Using the prompt_search_user_files_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileListDTO>, Integer, Hash)> prompt_search_user_files_with_http_info(query)

```ruby
begin
  # Files for query.
  data, status_code, headers = api_instance.prompt_search_user_files_with_http_info(query)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileListDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->prompt_search_user_files_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **query** | **String** | Query. |  |

### Return type

[**FileListDTO**](FileListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_by_folder_with_taggrams

> <Array<RecordingMinimalWithTaggramsDTO>> recordings_by_folder_with_taggrams(folder_name, opts)

Timeseries of AI generated moods, musical features and more for recordings in your folder.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
folder_name = 'Default' # String | Folder name
opts = {
  category_name: 'instrument', # String | Show only taggrams for one category.
  tag_name: 'energetic', # String | Show only taggrams for one tag.
  genre_name: 'Ska', # String | Show only taggrams for one genre.
  from_timestamp: 16.0, # Float | Show only taggrams data starting from from this timestamp in seconds.
  to_timestamp: 32.0, # Float | Show only taggrams data before this timestamp in seconds.
  fill_with_zero: true, # Boolean | If set to true, empty timeseries are filled with timeseries of 0.0 values.
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # Timeseries of AI generated moods, musical features and more for recordings in your folder.
  result = api_instance.recordings_by_folder_with_taggrams(folder_name, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->recordings_by_folder_with_taggrams: #{e}"
end
```

#### Using the recordings_by_folder_with_taggrams_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMinimalWithTaggramsDTO>>, Integer, Hash)> recordings_by_folder_with_taggrams_with_http_info(folder_name, opts)

```ruby
begin
  # Timeseries of AI generated moods, musical features and more for recordings in your folder.
  data, status_code, headers = api_instance.recordings_by_folder_with_taggrams_with_http_info(folder_name, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMinimalWithTaggramsDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->recordings_by_folder_with_taggrams_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **folder_name** | **String** | Folder name |  |
| **category_name** | **String** | Show only taggrams for one category. | [optional] |
| **tag_name** | **String** | Show only taggrams for one tag. | [optional] |
| **genre_name** | **String** | Show only taggrams for one genre. | [optional] |
| **from_timestamp** | **Float** | Show only taggrams data starting from from this timestamp in seconds. | [optional] |
| **to_timestamp** | **Float** | Show only taggrams data before this timestamp in seconds. | [optional] |
| **fill_with_zero** | **Boolean** | If set to true, empty timeseries are filled with timeseries of 0.0 values. | [optional] |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**Array&lt;RecordingMinimalWithTaggramsDTO&gt;**](RecordingMinimalWithTaggramsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordings_by_folder_with_tagstrengths

> <Array<RecordingMinimalWithTagstrengthsDTO>> recordings_by_folder_with_tagstrengths(folder_name, opts)

Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
folder_name = 'Default' # String | Folder name
opts = {
  category_name: 'instrument', # String | Show only taggrams for one category.
  tag_name: 'energetic', # String | Show only taggrams for one tag.
  genre_name: 'Ska', # String | Show only taggrams for one genre.
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
  result = api_instance.recordings_by_folder_with_tagstrengths(folder_name, opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->recordings_by_folder_with_tagstrengths: #{e}"
end
```

#### Using the recordings_by_folder_with_tagstrengths_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<RecordingMinimalWithTagstrengthsDTO>>, Integer, Hash)> recordings_by_folder_with_tagstrengths_with_http_info(folder_name, opts)

```ruby
begin
  # Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
  data, status_code, headers = api_instance.recordings_by_folder_with_tagstrengths_with_http_info(folder_name, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<RecordingMinimalWithTagstrengthsDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->recordings_by_folder_with_tagstrengths_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **folder_name** | **String** | Folder name |  |
| **category_name** | **String** | Show only taggrams for one category. | [optional] |
| **tag_name** | **String** | Show only taggrams for one tag. | [optional] |
| **genre_name** | **String** | Show only taggrams for one genre. | [optional] |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 20] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**Array&lt;RecordingMinimalWithTagstrengthsDTO&gt;**](RecordingMinimalWithTagstrengthsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## sign_up

> <SignUpDTO> sign_up(save_user_dto)

Sign up a new user.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
save_user_dto = SongtradrApiClientRuby::SaveUserDTO.new({email_address: 'email_address_example'}) # SaveUserDTO | 

begin
  # Sign up a new user.
  result = api_instance.sign_up(save_user_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->sign_up: #{e}"
end
```

#### Using the sign_up_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SignUpDTO>, Integer, Hash)> sign_up_with_http_info(save_user_dto)

```ruby
begin
  # Sign up a new user.
  data, status_code, headers = api_instance.sign_up_with_http_info(save_user_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SignUpDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->sign_up_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **save_user_dto** | [**SaveUserDTO**](SaveUserDTO.md) |  |  |

### Return type

[**SignUpDTO**](SignUpDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## token

> <JwtTokenDTO> token(token_request)

Generates a new JWT token for the given refresh token

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
token_request = SongtradrApiClientRuby::TokenRequest.new({refresh_token: 'refresh_token_example'}) # TokenRequest | 

begin
  # Generates a new JWT token for the given refresh token
  result = api_instance.token(token_request)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->token: #{e}"
end
```

#### Using the token_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JwtTokenDTO>, Integer, Hash)> token_with_http_info(token_request)

```ruby
begin
  # Generates a new JWT token for the given refresh token
  data, status_code, headers = api_instance.token_with_http_info(token_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JwtTokenDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->token_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **token_request** | [**TokenRequest**](TokenRequest.md) |  |  |

### Return type

[**JwtTokenDTO**](JwtTokenDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## update_password

> Object update_password(update_password_dto)

Update password by using the password reset token

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
update_password_dto = SongtradrApiClientRuby::UpdatePasswordDTO.new({token: 'token_example', password: 'password_example'}) # UpdatePasswordDTO | 

begin
  # Update password by using the password reset token
  result = api_instance.update_password(update_password_dto)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->update_password: #{e}"
end
```

#### Using the update_password_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> update_password_with_http_info(update_password_dto)

```ruby
begin
  # Update password by using the password reset token
  data, status_code, headers = api_instance.update_password_with_http_info(update_password_dto)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->update_password_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **update_password_dto** | [**UpdatePasswordDTO**](UpdatePasswordDTO.md) |  |  |

### Return type

**Object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/hal+json, application/json


## user_file

> <FileWIthUrlDTO> user_file(object_key)

Details and a download link for a file.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
object_key = '73818371-0963-412e-aa3d-27c2bab952a3' # String | ObjectKey of the file that should be edited.

begin
  # Details and a download link for a file.
  result = api_instance.user_file(object_key)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_file: #{e}"
end
```

#### Using the user_file_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileWIthUrlDTO>, Integer, Hash)> user_file_with_http_info(object_key)

```ruby
begin
  # Details and a download link for a file.
  data, status_code, headers = api_instance.user_file_with_http_info(object_key)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileWIthUrlDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_file_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **object_key** | **String** | ObjectKey of the file that should be edited. |  |

### Return type

[**FileWIthUrlDTO**](FileWIthUrlDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## user_files

> <FileListDTO> user_files(opts)

List and search your own files.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
opts = {
  isrc: 'USUM71703692', # String | Search for a ISRC
  contributor: 'Rick Rubin', # String | Search for a name that was involved as any contributor.
  main_artist: 'The Beatles', # String | Search for a main artist.
  composer: 'John Cale', # String | Search for a composer.
  title: 'Highway To Hell', # String | Search for a title.
  party_and_title: 'The Beatles yesterday', # String | Search for party and title.
  language: 'en', # String | Search for a language of the lyrics.
  genre_names: ['inner_example'], # Array<String> | 
  tag_names: ['inner_example'], # Array<String> | 
  release_date: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  primary_mood_cluster: 'aggressive', # String | 
  secondary_mood_cluster: 'aggressive', # String | 
  tertiary_mood_cluster: 'aggressive', # String | 
  valence: 'very sad', # String | 
  arousal: 'very calm', # String | 
  pleasantness: 'very unpleasant', # String | 
  engagement: 'very unengaging', # String | 
  vocals: 'instrumental', # String | 
  dominant_instrument: 'piano', # String | 
  secondary_instrument: 'piano', # String | 
  tertiary_instrument: 'piano', # String | 
  energy: 'very quiet', # String | 
  sound_generation: 'acoustic', # String | 
  tempo: 'very slow', # String | 
  scale: 'major key', # String | 
  key: 'C', # String | 
  rhythm: 'common time', # String | 
  primary_sound_character: 'aggressive', # String | 
  timbre: 'very warm', # String | 
  roughness: 'very clear', # String | 
  tonality: 'monotonous', # String | 
  harmony: 'very dissonant', # String | 
  texture: 'very thin', # String | 
  groovyness: 'very steady', # String | 
  space: 'very compact', # String | 
  loudness: 'very low', # String | 
  production_rating: 'low production quality', # String | 
  performance_rating: 'low performance quality', # String | 
  song_rating: 'low song quality', # String | 
  audience_age: 'Generation Z', # String | 
  audience_region: 'Australia and New Zealand', # String | 
  audience_gender: 'male', # String | 
  origin_decade: 'pre-1950s', # String | 
  curateability: 'curateable', # String | 
  use_case: 'background', # String | 
  channel_suitability: 'Spotify', # String | 
  similar_to_recording: 'similar_to_recording_example', # String | 
  songtradr_track_id: 'songtradr_track_id_example', # String | 
  usage_name: 'usage_name_example', # String | 
  bpm_min: 50, # Integer | Search for a minimal bpm.
  bpm_max: 210, # Integer | Search for a maximal bpm.
  name: 'Groove.mp3', # String | Search for a file name.
  folder: 'defaultFolder', # String | Search for a folder.
  extension: '.mp3', # String | Search for a file extension.
  upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  min_upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  max_upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  fingerprint_status: 'done', # String | Search for a fingerprint status.
  inference_status: 'done', # String | Search for a inference status.
  page: 56, # Integer | Zero-based page index (0..N)
  size: 56, # Integer | The size of the page to be returned
  sort: ['inner_example'] # Array<String> | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.
}

begin
  # List and search your own files.
  result = api_instance.user_files(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files: #{e}"
end
```

#### Using the user_files_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileListDTO>, Integer, Hash)> user_files_with_http_info(opts)

```ruby
begin
  # List and search your own files.
  data, status_code, headers = api_instance.user_files_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileListDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **isrc** | **String** | Search for a ISRC | [optional] |
| **contributor** | **String** | Search for a name that was involved as any contributor. | [optional] |
| **main_artist** | **String** | Search for a main artist. | [optional] |
| **composer** | **String** | Search for a composer. | [optional] |
| **title** | **String** | Search for a title. | [optional] |
| **party_and_title** | **String** | Search for party and title. | [optional] |
| **language** | **String** | Search for a language of the lyrics. | [optional] |
| **genre_names** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **tag_names** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **primary_mood_cluster** | **String** |  | [optional] |
| **secondary_mood_cluster** | **String** |  | [optional] |
| **tertiary_mood_cluster** | **String** |  | [optional] |
| **valence** | **String** |  | [optional] |
| **arousal** | **String** |  | [optional] |
| **pleasantness** | **String** |  | [optional] |
| **engagement** | **String** |  | [optional] |
| **vocals** | **String** |  | [optional] |
| **dominant_instrument** | **String** |  | [optional] |
| **secondary_instrument** | **String** |  | [optional] |
| **tertiary_instrument** | **String** |  | [optional] |
| **energy** | **String** |  | [optional] |
| **sound_generation** | **String** |  | [optional] |
| **tempo** | **String** |  | [optional] |
| **scale** | **String** |  | [optional] |
| **key** | **String** |  | [optional] |
| **rhythm** | **String** |  | [optional] |
| **primary_sound_character** | **String** |  | [optional] |
| **timbre** | **String** |  | [optional] |
| **roughness** | **String** |  | [optional] |
| **tonality** | **String** |  | [optional] |
| **harmony** | **String** |  | [optional] |
| **texture** | **String** |  | [optional] |
| **groovyness** | **String** |  | [optional] |
| **space** | **String** |  | [optional] |
| **loudness** | **String** |  | [optional] |
| **production_rating** | **String** |  | [optional] |
| **performance_rating** | **String** |  | [optional] |
| **song_rating** | **String** |  | [optional] |
| **audience_age** | **String** |  | [optional] |
| **audience_region** | **String** |  | [optional] |
| **audience_gender** | **String** |  | [optional] |
| **origin_decade** | **String** |  | [optional] |
| **curateability** | **String** |  | [optional] |
| **use_case** | **String** |  | [optional] |
| **channel_suitability** | **String** |  | [optional] |
| **similar_to_recording** | **String** |  | [optional] |
| **songtradr_track_id** | **String** |  | [optional] |
| **usage_name** | **String** |  | [optional] |
| **bpm_min** | **Integer** | Search for a minimal bpm. | [optional] |
| **bpm_max** | **Integer** | Search for a maximal bpm. | [optional] |
| **name** | **String** | Search for a file name. | [optional] |
| **folder** | **String** | Search for a folder. | [optional] |
| **extension** | **String** | Search for a file extension. | [optional] |
| **upload_end_time** | **Time** |  | [optional] |
| **min_upload_end_time** | **Time** |  | [optional] |
| **max_upload_end_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** | Search for a fingerprint status. | [optional] |
| **inference_status** | **String** | Search for a inference status. | [optional] |
| **page** | **Integer** | Zero-based page index (0..N) | [optional][default to 0] |
| **size** | **Integer** | The size of the page to be returned | [optional][default to 100] |
| **sort** | [**Array&lt;String&gt;**](String.md) | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] |

### Return type

[**FileListDTO**](FileListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## user_files_status

> <Array<FileSmallDTO>> user_files_status(object_keys)

Status details for files.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
object_keys = 'Example-objectKey' # String | Comma-separated  list of objectKeys of the files.

begin
  # Status details for files.
  result = api_instance.user_files_status(object_keys)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files_status: #{e}"
end
```

#### Using the user_files_status_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<FileSmallDTO>>, Integer, Hash)> user_files_status_with_http_info(object_keys)

```ruby
begin
  # Status details for files.
  data, status_code, headers = api_instance.user_files_status_with_http_info(object_keys)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<FileSmallDTO>>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files_status_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **object_keys** | **String** | Comma-separated  list of objectKeys of the files. |  |

### Return type

[**Array&lt;FileSmallDTO&gt;**](FileSmallDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## user_files_summary

> <FilesSummaryDTO> user_files_summary(opts)

Summary fo your files.

### Examples

```ruby
require 'time'
require 'songtradr_api_client_ruby'
# setup authorization
SongtradrApiClientRuby.configure do |config|
  # Configure Bearer authorization (JWT): bearer-jwt
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = SongtradrApiClientRuby::UserApi.new
opts = {
  isrc: 'USUM71703692', # String | Search for a ISRC
  contributor: 'Rick Rubin', # String | Search for a name that was involved as any contributor.
  main_artist: 'The Beatles', # String | Search for a main artist.
  composer: 'John Cale', # String | Search for a composer.
  title: 'Highway To Hell', # String | Search for a title.
  language: 'en', # String | Search for a language of the lyrics.
  genre_names: ['inner_example'], # Array<String> | 
  tag_names: ['inner_example'], # Array<String> | 
  release_date: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  primary_mood_cluster: 'aggressive', # String | 
  secondary_mood_cluster: 'aggressive', # String | 
  tertiary_mood_cluster: 'aggressive', # String | 
  valence: 'very sad', # String | 
  arousal: 'very calm', # String | 
  pleasantness: 'very unpleasant', # String | 
  engagement: 'very unengaging', # String | 
  vocals: 'instrumental', # String | 
  dominant_instrument: 'piano', # String | 
  secondary_instrument: 'piano', # String | 
  tertiary_instrument: 'piano', # String | 
  energy: 'very quiet', # String | 
  sound_generation: 'acoustic', # String | 
  tempo: 'very slow', # String | 
  scale: 'major key', # String | 
  key: 'C', # String | 
  rhythm: 'common time', # String | 
  primary_sound_character: 'aggressive', # String | 
  timbre: 'very warm', # String | 
  roughness: 'very clear', # String | 
  tonality: 'monotonous', # String | 
  harmony: 'very dissonant', # String | 
  texture: 'very thin', # String | 
  groovyness: 'very steady', # String | 
  space: 'very compact', # String | 
  loudness: 'very low', # String | 
  production_rating: 'low production quality', # String | 
  performance_rating: 'low performance quality', # String | 
  song_rating: 'low song quality', # String | 
  audience_age: 'Generation Z', # String | 
  audience_region: 'Australia and New Zealand', # String | 
  audience_gender: 'male', # String | 
  origin_decade: 'pre-1950s', # String | 
  curateability: 'curateable', # String | 
  use_case: 'background', # String | 
  channel_suitability: 'Spotify', # String | 
  similar_to_recording: 'Highway To Hell', # String | 
  songtradr_track_id: 'songtradr_track_id_example', # String | 
  usage_name: 'usage_name_example', # String | 
  bpm_min: 50, # Integer | Search for a minimal bpm.
  bpm_max: 210, # Integer | Search for a maximal bpm.
  name: 'Groove.mp3', # String | Search for a file name.
  folder: 'defaultFolder', # String | Search for a folder.
  extension: '.mp3', # String | Search for a file extension.
  upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  min_upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  max_upload_end_time: Time.parse('2013-10-20T19:20:30+01:00'), # Time | 
  fingerprint_status: 'done', # String | Search for a fingerprint status.
  inference_status: 'done' # String | Search for a inference status.
}

begin
  # Summary fo your files.
  result = api_instance.user_files_summary(opts)
  p result
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files_summary: #{e}"
end
```

#### Using the user_files_summary_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FilesSummaryDTO>, Integer, Hash)> user_files_summary_with_http_info(opts)

```ruby
begin
  # Summary fo your files.
  data, status_code, headers = api_instance.user_files_summary_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FilesSummaryDTO>
rescue SongtradrApiClientRuby::ApiError => e
  puts "Error when calling UserApi->user_files_summary_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **isrc** | **String** | Search for a ISRC | [optional] |
| **contributor** | **String** | Search for a name that was involved as any contributor. | [optional] |
| **main_artist** | **String** | Search for a main artist. | [optional] |
| **composer** | **String** | Search for a composer. | [optional] |
| **title** | **String** | Search for a title. | [optional] |
| **language** | **String** | Search for a language of the lyrics. | [optional] |
| **genre_names** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **tag_names** | [**Array&lt;String&gt;**](String.md) |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **primary_mood_cluster** | **String** |  | [optional] |
| **secondary_mood_cluster** | **String** |  | [optional] |
| **tertiary_mood_cluster** | **String** |  | [optional] |
| **valence** | **String** |  | [optional] |
| **arousal** | **String** |  | [optional] |
| **pleasantness** | **String** |  | [optional] |
| **engagement** | **String** |  | [optional] |
| **vocals** | **String** |  | [optional] |
| **dominant_instrument** | **String** |  | [optional] |
| **secondary_instrument** | **String** |  | [optional] |
| **tertiary_instrument** | **String** |  | [optional] |
| **energy** | **String** |  | [optional] |
| **sound_generation** | **String** |  | [optional] |
| **tempo** | **String** |  | [optional] |
| **scale** | **String** |  | [optional] |
| **key** | **String** |  | [optional] |
| **rhythm** | **String** |  | [optional] |
| **primary_sound_character** | **String** |  | [optional] |
| **timbre** | **String** |  | [optional] |
| **roughness** | **String** |  | [optional] |
| **tonality** | **String** |  | [optional] |
| **harmony** | **String** |  | [optional] |
| **texture** | **String** |  | [optional] |
| **groovyness** | **String** |  | [optional] |
| **space** | **String** |  | [optional] |
| **loudness** | **String** |  | [optional] |
| **production_rating** | **String** |  | [optional] |
| **performance_rating** | **String** |  | [optional] |
| **song_rating** | **String** |  | [optional] |
| **audience_age** | **String** |  | [optional] |
| **audience_region** | **String** |  | [optional] |
| **audience_gender** | **String** |  | [optional] |
| **origin_decade** | **String** |  | [optional] |
| **curateability** | **String** |  | [optional] |
| **use_case** | **String** |  | [optional] |
| **channel_suitability** | **String** |  | [optional] |
| **similar_to_recording** | **String** |  | [optional] |
| **songtradr_track_id** | **String** |  | [optional] |
| **usage_name** | **String** |  | [optional] |
| **bpm_min** | **Integer** | Search for a minimal bpm. | [optional] |
| **bpm_max** | **Integer** | Search for a maximal bpm. | [optional] |
| **name** | **String** | Search for a file name. | [optional] |
| **folder** | **String** | Search for a folder. | [optional] |
| **extension** | **String** | Search for a file extension. | [optional] |
| **upload_end_time** | **Time** |  | [optional] |
| **min_upload_end_time** | **Time** |  | [optional] |
| **max_upload_end_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** | Search for a fingerprint status. | [optional] |
| **inference_status** | **String** | Search for a inference status. | [optional] |

### Return type

[**FilesSummaryDTO**](FilesSummaryDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

