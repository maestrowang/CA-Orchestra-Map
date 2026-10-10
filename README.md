# California Orchestra Map

An interactive map of California middle and high schools with an orchestra or string program, by city. It covers 1,292 schools in 366 cities.

The whole site is one file, `index.html`. The data and the county outlines are embedded in it, so there is nothing to build or install.

## Files

| File | What it is |
|---|---|
| `index.html` | The map. This is the only file the site needs. |
| `data/orchestra-programs.csv` | The same school list as a spreadsheet-friendly file, for anyone who wants the data. |
| `data/cities.csv` | The city coordinates used to place the circles. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

## Publish with GitHub Pages

1. Create a new public repository on GitHub, for example `california-orchestra-map`.
2. Upload everything in this folder to the repository (Add file > Upload files), keeping `index.html` at the top level.
3. Open Settings > Pages. Under "Build and deployment", set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, and save.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/california-orchestra-map/`.

## Sources and limits

- High school courses: UC A-G Course List, 2026-27, Visual & Performing Arts / Music, searched by course title.
- Middle schools, and a cross-check for public high schools: California Department of Education course enrollment file, 2018-19, course code 2303 Orchestra/symphony. This data is several years old, so some programs have opened or closed since.
- City and county names and coordinates: CDE public school directory. Each circle sits at the average location of that city's public schools, so it is accurate to the city, not to a school address.
- Private middle schools are not covered.
- County outlines: US Census Bureau cartographic boundaries, via the `us-atlas` package.

The map loads two typefaces from Google Fonts. If they are unavailable it falls back to system fonts.

Data compiled October 2026.
