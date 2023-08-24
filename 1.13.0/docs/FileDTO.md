# SongtradrApiClientRuby::FileDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Integer** |  |  |
| **name** | **String** |  |  |
| **object_key** | **String** |  |  |
| **folder** | **String** |  |  |
| **extension** | **String** | extension of the file |  |
| **url** | **String** |  | [optional] |
| **upload_start_time** | **Time** |  | [optional] |
| **upload_end_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** | status of the audio recognition | [optional] |
| **fingerprint_start_time** | **Time** |  | [optional] |
| **fingerprint_end_time** | **Time** |  | [optional] |
| **inference_status** | **String** | status of the auto-tagging | [optional] |
| **inference_start_time** | **Time** |  | [optional] |
| **inference_end_time** | **Time** |  | [optional] |
| **recording** | [**RecordingMediumDTO**](RecordingMediumDTO.md) |  | [optional] |
| **error_time** | **Time** |  | [optional] |
| **error_message** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FileDTO.new(
  id: null,
  name: null,
  object_key: null,
  folder: null,
  extension: null,
  url: null,
  upload_start_time: null,
  upload_end_time: null,
  fingerprint_status: null,
  fingerprint_start_time: null,
  fingerprint_end_time: null,
  inference_status: null,
  inference_start_time: null,
  inference_end_time: null,
  recording: null,
  error_time: null,
  error_message: null
)
```

