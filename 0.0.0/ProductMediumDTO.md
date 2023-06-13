# SongtradrApiClientRuby::ProductMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Time** |  | [optional] |
| **pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] |
| **parties** | [**Array&lt;ProductPartyDTO&gt;**](ProductPartyDTO.md) |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreMinimalDTO&gt;**](GenreMinimalDTO.md) |  | [optional] |
| **gtin** | **String** |  | [optional] |
| **grid** | **String** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **takedown_date** | **Time** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::ProductMediumDTO.new(
  duration: null,
  pline: null,
  parties: null,
  titles: null,
  genres: null,
  gtin: null,
  grid: null,
  release_date: null,
  takedown_date: null
)
```

