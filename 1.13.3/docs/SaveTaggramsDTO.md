# SongtradrApiClientRuby::SaveTaggramsDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **timestamps** | **Array&lt;Float&gt;** |  | [optional] |
| **level1_genre** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **level2_genre** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **song_rating** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **performance_rating** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **production_rating** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **mood_cluster** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **vocals** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **dominant_instrument** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **sound_generation** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **rhythm** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **tonality** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **audience_age** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **audience_gender** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **audience_region** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **origin_region** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **origin_decade** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **language_of_performance** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **arousal** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **valence** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **pleasantness** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **engagement** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **energy** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **timbre** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **roughness** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **harmony** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **texture** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **groovyness** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **space** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **curateability** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **use_case** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **social_media** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |
| **industry_suitability** | **Hash&lt;String, Array&lt;Float&gt;&gt;** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::SaveTaggramsDTO.new(
  timestamps: null,
  level1_genre: null,
  level2_genre: null,
  song_rating: null,
  performance_rating: null,
  production_rating: null,
  mood_cluster: null,
  vocals: null,
  dominant_instrument: null,
  sound_generation: null,
  rhythm: null,
  tonality: null,
  audience_age: null,
  audience_gender: null,
  audience_region: null,
  origin_region: null,
  origin_decade: null,
  language_of_performance: null,
  arousal: null,
  valence: null,
  pleasantness: null,
  engagement: null,
  energy: null,
  timbre: null,
  roughness: null,
  harmony: null,
  texture: null,
  groovyness: null,
  space: null,
  curateability: null,
  use_case: null,
  social_media: null,
  industry_suitability: null
)
```

