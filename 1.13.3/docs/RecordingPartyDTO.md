# SongtradrApiClientRuby::RecordingPartyDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **party** | [**PartySmallDTO**](PartySmallDTO.md) |  |  |
| **contributor_types** | [**Array&lt;ContributorTypeDTO&gt;**](ContributorTypeDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::RecordingPartyDTO.new(
  party: null,
  contributor_types: null
)
```

