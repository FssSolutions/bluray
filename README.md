# Blu-ray Collection Organizer

A single-file, interactive organizer for a Blu-ray movie collection. Open
`index.html` in any browser — no install, no server, works offline.

**Live site:** https://fsssolutions.github.io/bluray/
(served from the `gh-pages` branch via GitHub Pages — requires the repo to be
public, or a paid plan if private)

## What it shows

For each film you get the **IMDb-style basics** (year, director, cast, genre,
runtime, synopsis, rating) plus a dedicated **"Shot On" cinematography panel**:

- **Cameras** — the bodies used (Arri Alexa, Panavision, IMAX 65mm, etc.)
- **Lenses** — lens sets (Panavision Primo, Ultra Panavision 70, …)
- **Format / Film stock** — film vs digital, gauge (35mm / 65mm / IMAX), sensor
- **Resolution / Finish** — capture resolution and the digital-intermediate finish

## Features

- Searchable, sortable poster grid
- Filter by how it was shot: **Film / Digital / IMAX / Animated**
- Click any film for full detail; edit every field inline
- **Add a film by typing just the title** (see lookup behaviour below)
- Data saved in your browser (localStorage); **Export / Import** to a JSON backup
- Ships pre-loaded with 26 starter films, all four spec fields filled in

## Adding films / online lookup

Type a title and press Enter. The app then:

1. Checks the built-in database (your 26 starter films have full data, including
   the Shot On specs).
2. If not found and you've added a free API key (⚙ Setup), it pulls the
   **basics + poster** automatically from
   [The Movie Database](https://www.themoviedb.org).
3. The four **Shot On** fields have **no free public API anywhere**, so for new
   titles you fill those in by hand (they default to "Unknown" until you do).

The starter films' cinematography data is best-effort from general knowledge —
edit anything that's off; every field is editable.
