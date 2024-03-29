# Gacha

Discord CCG bot using [Discord4J](https://github.com/Discord4J/Discord4J) and [MongoDB](https://github.com/mongodb/mongo).

## Gacha Data Folder

Data loaded during boot is stored in the user folder (%USERPROFILE%/GachaData)

### Cards (cards.json)
Card data is stored in `cards.json`.

Images for cards are stored in `/cards`.

The naming pattern is `series_name` or `series_name_variant`.

The syntax for color fields is `r, g, b`.
The syntax for stats fields is `hp, df, at, mg`.

- `name` (string)
- `variant` (string)
- `series` (series) - The series this card is from (see `series.json`)
- `source` (string) - The URL for the original image of the card
- `tier` (integer) - Between 1 and 6
- `disabled` (boolean) - Whether this card can be used
- `frameColor` (color)
- `font` (string)
- `font_size` (integer)
- `font_color` (color)
- `archetype` (archetype)
- `stats` (stats)