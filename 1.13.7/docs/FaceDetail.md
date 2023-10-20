# SongtradrApiClientRuby::FaceDetail

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **bounding_box** | [**BoundingBox**](BoundingBox.md) |  | [optional] |
| **age_range** | [**AgeRange**](AgeRange.md) |  | [optional] |
| **smile** | [**Smile**](Smile.md) |  | [optional] |
| **eyeglasses** | [**Eyeglasses**](Eyeglasses.md) |  | [optional] |
| **sunglasses** | [**Sunglasses**](Sunglasses.md) |  | [optional] |
| **gender** | [**Gender**](Gender.md) |  | [optional] |
| **beard** | [**Beard**](Beard.md) |  | [optional] |
| **mustache** | [**Mustache**](Mustache.md) |  | [optional] |
| **eyes_open** | [**EyeOpen**](EyeOpen.md) |  | [optional] |
| **mouth_open** | [**MouthOpen**](MouthOpen.md) |  | [optional] |
| **emotions** | [**Array&lt;Emotion&gt;**](Emotion.md) |  | [optional] |
| **landmarks** | [**Array&lt;Landmark&gt;**](Landmark.md) |  | [optional] |
| **pose** | [**Pose**](Pose.md) |  | [optional] |
| **quality** | [**ImageQuality**](ImageQuality.md) |  | [optional] |
| **confidence** | **Float** |  | [optional] |
| **face_occluded** | [**FaceOccluded**](FaceOccluded.md) |  | [optional] |
| **eye_direction** | [**EyeDirection**](EyeDirection.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::FaceDetail.new(
  bounding_box: null,
  age_range: null,
  smile: null,
  eyeglasses: null,
  sunglasses: null,
  gender: null,
  beard: null,
  mustache: null,
  eyes_open: null,
  mouth_open: null,
  emotions: null,
  landmarks: null,
  pose: null,
  quality: null,
  confidence: null,
  face_occluded: null,
  eye_direction: null
)
```

