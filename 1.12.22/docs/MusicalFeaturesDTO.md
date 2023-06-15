# SongtradrApiClientRuby::MusicalFeaturesDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **space** | **String** | Search for space | [optional] |
| **arousal** | **String** | Search for an arousal | [optional] |
| **dominant_instrument** | **String** | Search for a dominant instrument | [optional] |
| **energy** | **String** | Search for energy | [optional] |
| **engagement** | **String** | Search for an engagement | [optional] |
| **groovyness** | **String** | Search for groovyness | [optional] |
| **harmony** | **String** | Search for a degree of harmoniousness | [optional] |
| **pleasantness** | **String** | Search for pleasantness | [optional] |
| **primary_mood_cluster** | **String** | Search for a language of the lyrics | [optional] |
| **primary_sound_character** | **String** | Search for a sound character | [optional] |
| **rhythm** | **String** | Search for rhythm | [optional] |
| **roughness** | **String** | Search for roughness | [optional] |
| **scale** | **String** | Search for a tonal scale | [optional] |
| **sound_generation** | **String** | Search for type of sound generation | [optional] |
| **tempo** | **String** | Search for tempo | [optional] |
| **texture** | **String** | Search for texture | [optional] |
| **timbre** | **String** | Search for timbre | [optional] |
| **tonality** | **String** | Search for tonality | [optional] |
| **valence** | **String** | Search for a valence | [optional] |
| **vocals** | **String** | Search for a vocal gender or instrumental songs | [optional] |
| **origin_decade** | **String** | Search for origin decade | [optional] |
| **language_of_performance** | **String** |  | [optional] |
| **primary_sound_character_affinity** | **Float** |  | [optional] |
| **tonality_affinity** | **Float** |  | [optional] |
| **bpm** | **Float** |  | [optional] |
| **production_rating** | **String** |  | [optional] |
| **production_rating_affinity** | **Float** |  | [optional] |
| **performance_rating** | **String** |  | [optional] |
| **performance_rating_affinity** | **Float** |  | [optional] |
| **song_rating** | **String** |  | [optional] |
| **song_rating_affinity** | **Float** |  | [optional] |
| **audience_age** | **String** |  | [optional] |
| **audience_age_affinity** | **Float** |  | [optional] |
| **secondary_audience_age** | **String** |  | [optional] |
| **secondary_audience_age_affinity** | **Float** |  | [optional] |
| **tertiary_audience_age** | **String** |  | [optional] |
| **tertiary_audience_age_affinity** | **Float** |  | [optional] |
| **audience_gender** | **String** |  | [optional] |
| **audience_gender_affinity** | **Float** |  | [optional] |
| **audience_region_affinity** | **Float** |  | [optional] |
| **secondary_audience_region** | **String** |  | [optional] |
| **secondary_audience_region_affinity** | **Float** |  | [optional] |
| **tertiary_audience_region** | **String** |  | [optional] |
| **tertiary_audience_region_affinity** | **Float** |  | [optional] |
| **origin_region** | **String** |  | [optional] |
| **origin_region_affinity** | **Float** |  | [optional] |
| **origin_decade_affinity** | **Float** |  | [optional] |
| **language_of_performance_affinity** | **Float** |  | [optional] |
| **curateability_affinity** | **Float** |  | [optional] |
| **use_case_affinity** | **Float** |  | [optional] |
| **industry_suitability** | **String** | Search for Industry suitability | [optional] |
| **industry_suitability_affinity** | **Float** |  | [optional] |
| **audience_region** | **String** |  | [optional] |
| **curateability** | **String** | Search for curatebility | [optional] |
| **use_case** | **String** | Search for use case | [optional] |
| **channel_suitability** | **String** | Search for social media suitability | [optional] |
| **primary_mood_cluster_affinity** | **Float** |  | [optional] |
| **secondary_mood_cluster** | **String** | Search for a language of the lyrics | [optional] |
| **secondary_mood_cluster_affinity** | **Float** |  | [optional] |
| **tertiary_mood_cluster** | **String** | Search for a language of the lyrics | [optional] |
| **tertiary_mood_cluster_affinity** | **Float** |  | [optional] |
| **vocals_affinity** | **Float** |  | [optional] |
| **dominant_instrument_affinity** | **Float** |  | [optional] |
| **secondary_instrument** | **String** | Search for a dominant instrument | [optional] |
| **secondary_instrument_affinity** | **Float** |  | [optional] |
| **tertiary_instrument** | **String** | Search for a dominant instrument | [optional] |
| **tertiary_instrument_affinity** | **Float** |  | [optional] |
| **sound_generation_affinity** | **Float** |  | [optional] |
| **rhythm_affinity** | **Float** |  | [optional] |
| **valence_affinity** | **Float** |  | [optional] |
| **arousal_affinity** | **Float** |  | [optional] |
| **pleasantness_affinity** | **Float** |  | [optional] |
| **engagement_affinity** | **Float** |  | [optional] |
| **energy_affinity** | **Float** |  | [optional] |
| **tempo_affinity** | **Float** |  | [optional] |
| **scale_affinity** | **Float** |  | [optional] |
| **timbre_affinity** | **Float** |  | [optional] |
| **roughness_affinity** | **Float** |  | [optional] |
| **harmony_affinity** | **Float** |  | [optional] |
| **texture_affinity** | **Float** |  | [optional] |
| **groovyness_affinity** | **Float** |  | [optional] |
| **space_affinity** | **Float** |  | [optional] |
| **key_affinity** | **Float** |  | [optional] |
| **channel_suitability_affinity** | **Float** |  | [optional] |
| **key** | **String** | Search for a harmonic key | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::MusicalFeaturesDTO.new(
  space: null,
  arousal: null,
  dominant_instrument: null,
  energy: null,
  engagement: null,
  groovyness: null,
  harmony: null,
  pleasantness: null,
  primary_mood_cluster: null,
  primary_sound_character: null,
  rhythm: null,
  roughness: null,
  scale: null,
  sound_generation: null,
  tempo: null,
  texture: null,
  timbre: null,
  tonality: null,
  valence: null,
  vocals: null,
  origin_decade: null,
  language_of_performance: null,
  primary_sound_character_affinity: null,
  tonality_affinity: null,
  bpm: null,
  production_rating: null,
  production_rating_affinity: null,
  performance_rating: null,
  performance_rating_affinity: null,
  song_rating: null,
  song_rating_affinity: null,
  audience_age: null,
  audience_age_affinity: null,
  secondary_audience_age: null,
  secondary_audience_age_affinity: null,
  tertiary_audience_age: null,
  tertiary_audience_age_affinity: null,
  audience_gender: null,
  audience_gender_affinity: null,
  audience_region_affinity: null,
  secondary_audience_region: null,
  secondary_audience_region_affinity: null,
  tertiary_audience_region: null,
  tertiary_audience_region_affinity: null,
  origin_region: null,
  origin_region_affinity: null,
  origin_decade_affinity: null,
  language_of_performance_affinity: null,
  curateability_affinity: null,
  use_case_affinity: null,
  industry_suitability: null,
  industry_suitability_affinity: null,
  audience_region: null,
  curateability: null,
  use_case: null,
  channel_suitability: null,
  primary_mood_cluster_affinity: null,
  secondary_mood_cluster: null,
  secondary_mood_cluster_affinity: null,
  tertiary_mood_cluster: null,
  tertiary_mood_cluster_affinity: null,
  vocals_affinity: null,
  dominant_instrument_affinity: null,
  secondary_instrument: null,
  secondary_instrument_affinity: null,
  tertiary_instrument: null,
  tertiary_instrument_affinity: null,
  sound_generation_affinity: null,
  rhythm_affinity: null,
  valence_affinity: null,
  arousal_affinity: null,
  pleasantness_affinity: null,
  engagement_affinity: null,
  energy_affinity: null,
  tempo_affinity: null,
  scale_affinity: null,
  timbre_affinity: null,
  roughness_affinity: null,
  harmony_affinity: null,
  texture_affinity: null,
  groovyness_affinity: null,
  space_affinity: null,
  key_affinity: null,
  channel_suitability_affinity: null,
  key: null
)
```

