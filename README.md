# Earth Information Jukebox — NASA GISTEMP v4 edition

## Genuine NASA data now included

**Global Temperature** loads verified NASA GISTEMP v4 *Land–Ocean Temperature Index* annual **J-D** anomalies, relative to the **1951–1980** mean, covering 1880–2025. The 2026 annual figure was omitted because the uploaded NASA source marks it incomplete (`***`). Data was taken from the user-provided official NASA CSV `GLB.Ts+dSST.csv`, preserving reported centidegree precision.

NASA source: https://data.giss.nasa.gov/gistemp/
Direct NASA data downloads: https://data.giss.nasa.gov/gistemp/data_v4.html

The website's **Global Temperature** button uses the NASA series by default without an upload step. The included `nasa-temperature.csv` provides a reusable year,value export. **Ocean Signals** and **Arctic Sea Ice** remain fictional illustrative demos and are labeled as such. The Earth globe is stylized artwork, not NASA Earth Information Center imagery. The generated audio is synthetic pitch mapping, not literal audio recorded from Earth.

## Publish to GitHub Pages

Upload these updated files into the ROOT of your existing GitHub repository `earth-information-jukebox`, replacing the old versions: `index.html`, `app.js`, `README.md`; add `nasa-temperature.csv`. The existing `styles.css` file is unchanged but may also be uploaded. Commit changes. Verify the public Pages URL and open the Global Temperature dataset.

## NASA project submission citation

**Link Text:** NASA GISS Surface Temperature Analysis (GISTEMP v4)

**Link URL:** https://data.giss.nasa.gov/gistemp/

Suggested truthful description: 'We integrated annual global land–ocean temperature anomaly data from NASA GISTEMP v4 (1880–2025), referenced to the 1951–1980 baseline, into the Global Temperature visualization and sonification. The Ocean and Arctic Ice modes remain illustrative. This is not an integration of NASA Earth Information Center visual frames.'

## Development

HTML, CSS, JavaScript, Canvas and Web Audio API; no external libraries required. Open index.html locally or deploy through GitHub Pages. Browser audio starts after user interaction.
