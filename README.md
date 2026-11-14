# Earth Information Jukebox — Website Prototype

A standalone, responsive website inspired by the **2026 NASA Space Apps Challenge: The Earth Information Jukebox**.

**IMPORTANT:** Built-in temperature, ocean, and ice series are **illustrative invented numbers**. The globe is procedural artwork, **not** Earth Information Center (EIC) imagery. No NASA API or live data is connected. The website is an independent prototype and is not endorsed by NASA.

## Cara buka (Windows)

1. Extract fail ZIP.
2. Buka folder `earth-information-jukebox`.
3. Double-click `index.html` untuk buka dalam Chrome atau Microsoft Edge.
4. Klik **Play soundscape** untuk aktifkan audio (browser memerlukan klik pengguna).
5. Cuba **Auto travel**, tukar dataset, atau upload fail `sample-data.csv`.

Untuk edit: buka folder ini di **VS Code**. Anda boleh gunakan Live Server, tetapi tidak wajib.

## Features

- Mobile-friendly visual design and artistic animated globe
- Three **demo-only** themed datasets
- Dynamic line chart, year slider, auto-play through time
- Real-time synthesized sound from Web Audio API; numerical values map to pitch
- Volume slider and mute toggle
- Import your own CSV dataset (`year,value`), sorted by year and limited to 500 rows / 1 MB
- No account, backend, database, API key, or paid packages needed

## Sound mapping

Each numerical data value is normalized between the minimum and maximum of the current dataset. The value maps onto a 16-semitone range above 174.61 Hz; stronger changes shorten each note. Sound is generated in the browser, so there are no premade recorded samples.

## How to improve for a real NASA submission

1. Visit the [official challenge](https://www.spaceappschallenge.org/2026/challenges/the-earth-information-jukebox/) and read its **Resources** section.
2. Select specific **NASA EIC / SVS visualization frames** and determine image permissions/credit requirements.
3. Find the matching **measured dataset** behind the selected visualization (e.g. from NASA archives) and document variable, units, location, time period, uncertainty, and citation.
4. Import the verified values via CSV and update labels, units, notes, bibliography, and visuals to match.
5. If you want true automatic synchronization between EIC frames and sound, add frame-by-frame time alignment and an appropriate data interface. The current version does **not** implement that integration.
6. Include a team name, presentation/demo video, and submission documentation as required by the challenge portal.

## Files

- `index.html` — page structure
- `styles.css` — theme and responsive layout
- `app.js` — datasets, chart, globe, CSV parsing, and audio
- `sample-data.csv` — **fictional test data** to verify import

## Credits & links

- Challenge: https://www.spaceappschallenge.org/2026/challenges/the-earth-information-jukebox/
- No NASA pictures, logos, or proprietary media are packaged.
- Optional Google Fonts are requested online; the site falls back to system fonts when offline.

This is a prototype, not an official NASA product or a completed scientific research submission.
