# Ocean Map Maker

A one-page tool for making presentation maps of Ocean's locations on the Ocean Mapbox style: upload a location spreadsheet, highlight countries, add one-off markers, and export slide-ready PNGs.

## Use it

Open the site, then:

1. **Locations:** drop in a CSV, Excel or GeoJSON file. Latitude/longitude columns are detected automatically (including the website export's "Map Lat" / "Map Lng"). For Ocean website exports, drafts and the duplicate `netherlands-dutch` rows are filtered out by default — see **Filters** on the dataset.
2. **Group by** a column such as City to show one circle per city, sized by number of sites.
3. **Country highlights:** search, click the map, or use "Highlight the countries in …" from the data.
4. **Extra markers:** search a place, type `lat, lng`, or click the map.
5. **Export:** pick a size, position the map inside the frame, and download or copy the PNG.

Use **Save project** to keep a map (data included) as a `.json` file and **Open project** to pick it up again.

`sample-locations.csv` is example data for trying the tool.

## Notes

- Place search uses OpenStreetMap Nominatim (one search per Enter, per its usage policy).
- Exported PNGs carry a small "© Mapbox © OpenStreetMap" credit, which Mapbox's terms expect on maps using its data.
- The Mapbox token in `index.html` is a public token. Restrict it to this site's address in the Mapbox account so it can't be reused elsewhere.
