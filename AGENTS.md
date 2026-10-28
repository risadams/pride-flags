# AGENTS.md

Pure-CSS library of LGBTQ+ pride flags, published as `@risadams/pride-flags`. Each flag is a `.flag.<name>` class that draws itself with CSS gradients. There is no JavaScript.

## Layout

- `src/pride-flags.scss`: the library source. Flat list of `.flag.<name>` rules, one `background:` each. Flags are grouped by category. Equal-band flags use the `stripes()` function with a list of colors, and `$rainbow` is shared by every rainbow-based flag.
- `src/demo.css`: styles for the demo page only. It is not shipped.
- `index.html`: demo page. One `<section>` per flag, grouped under category headers. Loads `src/demo.css` and `dist/pride-flags.min.css`.
- `dist/`: build output (`.css`, `.min.css`, and source maps). **Committed to git and published to npm** (`files: dist/*.css`).
- `README.md`: usage plus the categorized list of flag class names.
- `FLAGS.md`: where each flag's colors came from and whether they have been verified.
- `.github/workflows/build.yml`: CI that builds and fails if `dist/` is out of date.

## Commands

```sh
npm install
npm run build   # sass -> dist/pride-flags.css, then cleancss -> dist/pride-flags.min.css
```

There are no tests. CI only checks that `dist/` matches `src/`. To check a flag, build and open `index.html` through a local server (e.g. `python -m http.server`). Headless Chrome with `--screenshot` also works.

## Adding or changing a flag

1. Add or edit a `.flag.<kebab-case-name>` rule in `src/pride-flags.scss`. Equal bands are `stripes(#color1 #color2 ...)`, top to bottom. Unequal bands (bisexual, hijra) are written as hard-stop `linear-gradient`s. Shapes that gradients cannot draw (`doe`, `pocket-gender`, the bear paw) use an inline SVG data URI as a background layer. Keep these small. More complex flags layer `conic-gradient` or `radial-gradient` shapes (chevrons, triangles, rings) over a stripe base. Copy a similar existing flag.
2. Add a `<section>` to `index.html` under the right category. Copy an existing one. It needs `class="flag <name>" role="img"` and a descriptive `aria-label` that gives the flag's name, then its stripes and shapes in order, with colors.
3. Add the class name to the matching category list in `README.md`. Lists are alphabetical.
4. Record the color source in `FLAGS.md`, and mark it unverified if it is not from a reference.
5. Run `npm run build` and commit the regenerated `dist/` files with the source change.

## Conventions

- The base `.flag` is `300px` wide with `aspect-ratio: 14 / 9`. The `.icon` modifier (with `.large` and `.small` sizes) makes a small inline version. Flags with text or shapes sized in `cqw` (`polyamory`, `polyamorous-new`) are container-query containers, so they scale with the flag and need no icon overrides.
- Name classes in kebab-case, and keep them identical in the SCSS, the HTML and the README.
- `.editorconfig` sets 2-space indent, LF line endings, UTF-8 and a final newline.
- Never hand-edit `dist/`. Change `src/` and rebuild.
- Flags must always carry `role="img"` and an `aria-label` in demos and docs, so the accessibility text is part of any flag change.
- Do not guess colors. Use a published reference (prideflags.org SVGs first; see `FLAGS.md`) and update `FLAGS.md`.
- Version bumps and publishing are the maintainer's job. Do not change `package.json` version.
