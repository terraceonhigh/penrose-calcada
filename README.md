# Penrose Calcada

Interactive aperiodic Penrose tiling generator inspired by Portuguese calçada pavement.

**[Live demo](https://terraceonhigh.github.io/penrose-calcada/)**

---

## What it does

Generates gap-free Penrose tilings using Robinson triangle subdivision, rendered on an HTML canvas. Each page load produces a unique tiling via random rotation. No dependencies — a single HTML file.

## Features

- **Penrose P3 tiling** via recursive Robinson triangle decomposition
- **Colouring rules:** triangle type, thick/thin rhombus, outlines only, alternating, star detection, calçada random
- **Theme support:** 5 built-in colour schemes (dark, azulejo, azulejo-dark, calçada, calçada-dark)
- **Interactive controls:** subdivisions, scale, opacity, border style
- **Rhombus pairing:** triangles are paired into proper thick and thin Penrose rhombi
- **Star detection:** identifies 5-fold star formations in the tiling

## Usage

Open `index.html` in a browser. No build step, no server required.

## Algorithm

1. Start with 10 golden triangles arranged in a decagonal sun pattern
2. Recursively subdivide using Robinson triangle rules (golden ratio proportions)
3. Pair adjacent triangles sharing a hypotenuse into rhombi
4. Render with chosen colouring and border rules

The golden ratio phi = (1 + sqrt(5)) / 2 governs the subdivision proportions, guaranteeing aperiodicity.

## Calçada connection

[Calçada portuguesa](https://en.wikipedia.org/wiki/Portuguese_pavement) is the traditional pavement art found across Portugal — hand-laid limestone and basalt cobblestones forming geometric and figurative patterns. This generator captures the two-tone, tessellated aesthetic in an aperiodic mathematical form.

## License

MIT
