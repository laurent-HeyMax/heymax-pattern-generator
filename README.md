# Pattern generator

A brand pattern generator built from the mark. Generates non-overlapping
compositions using four layouts and exports print-ready vectors and raster.

**Live demo:** https://laurent-heymax.github.io/heymax-pattern-generator/

## Patterns

- **Grid** — complete rectangular grid, evenly margined.
- **Fibonacci spiral** — phyllotaxis layout, spacing derived from the true nearest-neighbour distance.
- **Perlin flow field** — a grid where each mark rotates to follow a noise field.
- **Concentric circles** — rings spaced so both arc and radial gaps stay clear.
- **Halftone** — mark size fades with radial distance and noise, like a dot-screen.
- **Waves** — size and rotation ripple across rows in sine phase.
- **Orbit rings** — concentric rings with tangent-rotated marks and alternating phase.
- **Diagonal cascade** — size and rotation graded along the diagonal.

Every layout sizes its elements from its own spacing, so marks never overlap.

## Controls

- Pattern, count, element size, spread, rotation
- Turbulence / wave detail and effect strength (per pattern)
- Colour modes: single, brand ramp
- Brand pairing swatches, background / element colour, opacity
- Shuffle seed for noise-driven layouts

## Export

- **SVG** — flattened 1080px vectors (each mark a real `<path>`), opens correctly in Figma and Illustrator.
- **PNG** — 2160px raster for social and retina use.

## Run

No build step, no dependencies. Either:

- Open `index.html` directly in a browser, or
- Serve locally: `python3 -m http.server` then open http://localhost:8000

## License

MIT
