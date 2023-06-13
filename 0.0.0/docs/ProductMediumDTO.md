# SongtradrApiClientRuby::ProductMediumDTO

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **duration** | **Time** |  | [optional] |
| **parties** | [**Array&lt;ProductPartyDTO&gt;**](ProductPartyDTO.md) |  | [optional] |
| **grid** | **String** |  | [optional] |
| **release_date** | **Time** |  | [optional] |
| **takedown_date** | **Time** |  | [optional] |
| **pline** | [**PLineDTO**](PLineDTO.md) |  | [optional] |
| **titles** | [**Array&lt;TitleDTO&gt;**](TitleDTO.md) |  | [optional] |
| **genres** | [**Array&lt;GenreMinimalDTO&gt;**](GenreMinimalDTO.md) |  | [optional] |
| **gtin** | **String** |  | [optional] |

## Example

```ruby
require 'songtradr_api_client_ruby'

instance = SongtradrApiClientRuby::ProductMediumDTO.new(
  duration: null,
  parties: null,
  grid: null,
  release_date: null,
  takedown_date: null,
  pline: null,
  titles: null,
  genres: null,
  gtin: null
)
```

