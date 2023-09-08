# SongtradrApiClientRuby::TagstrengthDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **strength** | **Float** | Strength of presence of the corresponding category, tag or genre. |  |
| **category_name** | **String** |  |  |
| **tag_name** | **String** |  | [optional] |
| **genre_name** | **String** |  | [optional] |
| **scale** | **Array&lt;Integer&gt;** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::TagstrengthDTO.new(
  strength: null,
  category_name: null,
  tag_name: null,
  genre_name: null,
  scale: null
)
```

