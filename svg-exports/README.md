# Year-by-year SVG exports

13 files, one per checkpoint year (every 5 years from 1967, plus the final 2024
state): `year-1967.svg`, `year-1972.svg`, `year-1977.svg`, `year-1982.svg`,
`year-1987.svg`, `year-1992.svg`, `year-1997.svg`, `year-2002.svg`,
`year-2007.svg`, `year-2012.svg`, `year-2017.svg`, `year-2022.svg`,
`year-2024.svg`.

These are true vector SVGs (not screenshots) — every point and the boundary
line is a real, editable SVG element (`<circle>`, `<path>`), generated
directly from the underlying geographic data (equirectangular projection, not
Esri/Google Mercator — close enough for reference at this scale, but position
will drift slightly if pasted over a Mercator-projected basemap image).

## What's in each file
- **Dashed line**: the Green Line (1949 Armistice Line / West Bank boundary)
- **Pink circles** (`#EB0EA5`): settlements founded by that year
- **Blue circles** (`#00BAFC`): outposts founded by that year
- **Gray circles** (`#9AA0A6`): farms/industrial areas/other — shown at all
  times since the source data has no founding year for these
- **Year label**, bottom-left, in Playfair Display / `#004E79` (The National's
  brand serif + primary blue)

All layers are grouped (`<g id="...">`) so they can be toggled/recolored
independently in Illustrator/After Effects.

## Not included (add separately, once, not per-file)
- The "Data Explained" kicker mark, headline, legend and source attribution —
  these don't change per year, see the live interactive build one level up
  (`../index.html`) for their exact styling.
- A real basemap (roads, place names, terrain) — these SVGs are data-only,
  meant to be composited over whatever basemap the final piece uses.

## Source
Data: Peace Now (GIS layers, updated Nov 2024). Canvas bounds match AP's own
interactive graphic exactly (34.666436, 31.281522 – 35.721123, 32.711658).
