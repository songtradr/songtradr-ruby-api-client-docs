# SongtradrApiClientRuby::Label

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **confidence** | **Float** |  | [optional] |
| **instances** | [**Array&lt;Instance&gt;**](Instance.md) |  | [optional] |
| **parents** | [**Array&lt;Parent&gt;**](Parent.md) |  | [optional] |
| **aliases** | [**Array&lt;LabelAlias&gt;**](LabelAlias.md) |  | [optional] |
| **categories** | [**Array&lt;LabelCategory&gt;**](LabelCategory.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::Label.new(
  name: null,
  confidence: null,
  instances: null,
  parents: null,
  aliases: null,
  categories: null
)
```

