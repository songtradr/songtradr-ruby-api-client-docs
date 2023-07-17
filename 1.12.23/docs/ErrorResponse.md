# SongtradrApiClientRuby::ErrorResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **timestamp** | **Time** | timestamp |  |
| **status** | **Integer** | HTTP Status code |  |
| **error** | **String** | HTTP status message |  |
| **message** | **String** | detailed error message | [optional] |
| **path** | **String** | path of the called API endpoint | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::ErrorResponse.new(
  timestamp: null,
  status: null,
  error: null,
  message: null,
  path: null
)
```

