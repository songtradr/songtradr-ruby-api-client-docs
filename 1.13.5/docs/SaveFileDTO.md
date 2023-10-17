# SongtradrApiClientRuby::SaveFileDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **folder** | **String** |  | [optional] |
| **extension** | **String** |  | [optional] |
| **object_key** | **String** |  | [optional] |
| **customer** | **String** |  | [optional] |
| **upload_start_time** | **Time** |  | [optional] |
| **upload_end_time** | **Time** |  | [optional] |
| **fingerprint_status** | **String** |  | [optional] |
| **fingerprint_start_time** | **Time** |  | [optional] |
| **fingerprint_end_time** | **Time** |  | [optional] |
| **inference_status** | **String** |  | [optional] |
| **inference_start_time** | **Time** |  | [optional] |
| **inference_end_time** | **Time** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::SaveFileDTO.new(
  name: null,
  folder: null,
  extension: null,
  object_key: null,
  customer: null,
  upload_start_time: null,
  upload_end_time: null,
  fingerprint_status: null,
  fingerprint_start_time: null,
  fingerprint_end_time: null,
  inference_status: null,
  inference_start_time: null,
  inference_end_time: null
)
```

