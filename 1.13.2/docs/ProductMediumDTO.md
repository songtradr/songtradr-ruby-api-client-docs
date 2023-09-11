# SongtradrApiClientRuby::ProductMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Time** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **takedown_date** | **Time** |  | [optional] |
| **parties** | [**Array&lt;ProductPartyDTO&gt;**](ProductPartyDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreMinimalDTO&gt;**](GenreMinimalDTO.md) |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **gtin** | **String** |  | [optional] |
| **grid** | **String** |  | [optional] |
| **pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::ProductMediumDTO.new(
  duration: null,
  release_date: null,
  takedown_date: null,
  parties: null,
  genres: null,
  titles: null,
  gtin: null,
  grid: null,
  pline: null
)
```

