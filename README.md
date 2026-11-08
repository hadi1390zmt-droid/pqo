# SOLARIS — Interactive Solar System Atlas

A bilingual Persian/English cinematic Solar System website built with separate HTML, CSS and JavaScript files.

## Run locally
Because the JavaScript uses ES modules, open the folder with a local static server rather than opening `index.html` directly.

### Python
```bash
cd solaris
python -m http.server 8000
```
Then visit http://localhost:8000

### Node
```bash
npx serve .
```

## Features
- Responsive OLED-inspired dark interface
- Persian/English language toggle (RTL/LTR)
- Interactive schematic orbital model with pause/resume
- Planet selector and searchable/filterable body catalog
- Science dossier dialog for each included world
- Surface-weight calculator using approximate surface gravity
- Ideal circular Earth-orbit speed calculator
- Mission highlights

## Scientific scope and caveats
- The orbital view is illustrative and explicitly **not to scale**. Orbital radii, body sizes and animation periods are stylized for legibility.
- Values are rounded reference values. Moon counts and some physical parameters can change as discoveries are confirmed.
- The circular-orbit calculator uses Earth's standard gravitational parameter and assumes a point-mass Earth and an ideal circular orbit. It does not model atmospheric drag, oblateness, perturbations or launch constraints.
- Surface gravity is an approximate reference value; gas giants do not have a solid surface in the ordinary terrestrial sense.
- This is an educational starter atlas, not an exhaustive database of every known moon, asteroid, comet, trans-Neptunian object or research result.

## Data references for future expansion
Use primary sources and cite datasets in the UI when adding precise or time-sensitive values:
- NASA Solar System Exploration: https://solarsystem.nasa.gov/
- NASA Planetary Fact Sheet: https://nssdc.gsfc.nasa.gov/planetary/factsheet/
- JPL Solar System Dynamics: https://ssd.jpl.nasa.gov/
- International Astronomical Union (planet definition): https://www.iau.org/
