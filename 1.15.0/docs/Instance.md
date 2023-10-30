# SongtradrApiClientRuby::Instance

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **bounding_box** | [**BoundingBox**](BoundingBox.md) |  | [optional] |
| **confidence** | **Float** |  | [optional] |
| **dominant_colors** | [**Array&lt;DominantColor&gt;**](DominantColor.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::Instance.new(
  bounding_box: null,
  confidence: null,
  dominant_colors: null
)
```

