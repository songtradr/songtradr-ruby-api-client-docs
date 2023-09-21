# SongtradrApiClientRuby::FileSmallDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  |  |
| **id** | **Integer** |  |  |
| **extension** | **String** | extension of the file |  |
| **error_message** | **String** |  | [optional] |
| **folder** | **String** |  |  |
| **object_key** | **String** |  |  |
| **upload_start_time** | **Time** |  | [optional] |
| **upload_end_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** | status of the audio recognition | [optional] |
| **fingerprint_start_time** | **Time** |  | [optional] |
| **fingerprint_end_time** | **Time** |  | [optional] |
| **inference_status** | **String** | status of the auto-tagging | [optional] |
| **inference_start_time** | **Time** |  | [optional] |
| **inference_end_time** | **Time** |  | [optional] |
| **error_time** | **Time** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FileSmallDTO.new(
  name: null,
  id: null,
  extension: null,
  error_message: null,
  folder: null,
  object_key: null,
  upload_start_time: null,
  upload_end_time: null,
  fingerprint_status: null,
  fingerprint_start_time: null,
  fingerprint_end_time: null,
  inference_status: null,
  inference_start_time: null,
  inference_end_time: null,
  error_time: null
)
```

