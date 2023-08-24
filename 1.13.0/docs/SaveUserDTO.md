# SongtradrApiClientRuby::SaveUserDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **system** | **String** |  | [optional] |
| **email_address** | **String** |  |  |
| **password** | **String** |  | [optional] |
| **full_name** | **String** |  | [optional] |
| **company_name** | **String** |  | [optional] |
| **language** | **String** | Current status of the recording. | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::SaveUserDTO.new(
  system: null,
  email_address: null,
  password: null,
  full_name: null,
  company_name: null,
  language: null
)
```

