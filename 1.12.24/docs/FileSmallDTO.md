# SongtradrApiClientRuby::FileSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **id** | **Integer** |  |  |
| **extension** | **String** | extension of the file |  |
| **error_message** | **String** |  | [optional] |
| **error_time** | **Time** |  | [optional] |
| **fingerprint_end_time** | **Time** |  | [optional] |
| **inference_start_time** | **Time** |  | [optional] |
| **fingerprint_start_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** | status of the audio recognition | [optional] |
| **inference_status** | **String** | status of the auto-tagging | [optional] |
| **inference_end_time** | **Time** |  | [optional] |
| **folder** | **String** |  |  |
| **upload_end_time** | **Time** |  | [optional] |
| **upload_start_time** | **Time** |  | [optional] |
| **object_key** | **String** |  |  |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FileSmallDTO.new(
  name: null,
  id: null,
  extension: null,
  error_message: null,
  error_time: null,
  fingerprint_end_time: null,
  inference_start_time: null,
  fingerprint_start_time: null,
  fingerprint_status: null,
  inference_status: null,
  inference_end_time: null,
  folder: null,
  upload_end_time: null,
  upload_start_time: null,
  object_key: null
)
```

