# AGENTS.md

## Cursor Cloud specific instructions

This is a static portfolio site (vanilla HTML/CSS/JS) with **zero dependencies** and **no build step**. The entire application lives in `index.html`.

### Running the dev server

```bash
python3 -m http.server 3000
# Site available at http://localhost:3000
```

Any static file server works. There is no package manager, framework, or build tool.

### No lint / test / build

- No linter, test framework, or CI/CD is configured.
- No `package.json`, `Makefile`, or dependency manifests exist.
- Validation is purely manual: open the site in a browser and verify sections render and interactive features (nav scroll, music player, particle canvas) work.

### Key interactive features to test

- **Smooth scroll navigation** via nav links (About, Experience, Open Source, Apps, Contact)
- **Generative lo-fi music player** (bottom-right corner) — click the spinning disc to toggle
- **Canvas particle background** with mouse repulsion
- **Scroll-reveal animations** via Intersection Observer
- **Animated stat counters** in the hero section
