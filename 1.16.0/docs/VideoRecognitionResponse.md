# SongtradrApiClientRuby::VideoRecognitionResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **labels** | [**Array&lt;LabelDetection&gt;**](LabelDetection.md) |  | [optional] |
| **faces** | [**Array&lt;FaceDetection&gt;**](FaceDetection.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::VideoRecognitionResponse.new(
  labels: null,
  faces: null
)
```

