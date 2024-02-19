# SongtradrApiClientRuby::JwtTokenDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **jwt_token** | **String** |  |  |
| **expiration_date** | **Time** |  |  |
| **refresh_token** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::JwtTokenDTO.new(
  jwt_token: null,
  expiration_date: null,
  refresh_token: null
)
```

