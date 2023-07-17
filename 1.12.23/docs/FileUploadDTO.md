# SongtradrApiClientRuby::FileUploadDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **identifiers** | [**Array&lt;ConfigIdentifierDTO&gt;**](ConfigIdentifierDTO.md) |  | [optional] |
| **flags** | **Array&lt;String&gt;** |  | [optional] |
| **access** | [**Array&lt;ConfigAccessDTO&gt;**](ConfigAccessDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FileUploadDTO.new(
  identifiers: null,
  flags: null,
  access: null
)
```

