# CSS Pride Flags

![npm](https://img.shields.io/npm/v/@risadams/pride-flags)

## Install

This is a pure CSS library that can be included in your project to display LGBT+ pride flags as either large images, or small icons. It should be straightforward to install and use, and will be updated with new options and flags as they become available.

```sh
npm install @risadams/pride-flags
```

Import `@risadams/pride-flags` in a bundler, or link `node_modules/@risadams/pride-flags/dist/pride-flags.min.css`.

## Usage

```html
<head>
  <link rel="stylesheet" href="dist/pride-flags.min.css" />
</head>

<body>
  <div class="flag progress" role="img" aria-label="Progress Pride Flag"></div>
  <div class="flag icon progress" role="img" aria-label="Progress Pride Flag"></div>
</body>
```

Flags are drawn with CSS, so they have no text of their own. Give each one `role="img"` and an `aria-label`.

## Flag Options

All flags with examples can be seen in this post: https://risadams.com/blog/2025/05/05/new-project-release-pride-flags

### Traditional/Historical Pride Flags

- ally-pride
- gilbert-baker
- intersex-inclusive
- new-pride
- philadelphia
- pink-triangle
- pride-1978
- pride-of-africa
- progress
- queer
- social-justice
- traditional

### Gender Identity Flags

- agender
- androgyne
- bigender
- bxy
- demiboy
- demigender
- demigirl
- gendercreative
- genderfluid
- genderflux
- genderqueer
- gxrl
- hijra
- littlefluid
- metagender
- neutrois
- nxnbinary
- nonbinary
- pangender
- transgender
- unlabeled

### Sexual Orientation Flags

- abrosexual
- asexual
- bisexual
- demisexual
- gay-men
- graysexual
- lesbian
- lipstick-lesbian
- omnisexual
- pansexual
- polysexual
- sapphic
- twink

### Romantic Orientation Flags

- aromantic (`aromantic-spectrum` is an alias)
- demiromantic

### Relationship Structure Flags

- polyamory (blue, red and black with a yellow π)
- polyamorous-new (2022 tricolor with a white chevron and gold heart)

### Community/Cultural Flags

- bear-brotherhood
- drag
- intersex
- labrys
- leather
- puppy
- rubber
- trans-inclusive

### Spectrum Flags

- aromantic-spectrum
- asexual-spectrum

## Accuracy

[FLAGS.md](FLAGS.md) lists which flags have been checked against a reference and which have not. Corrections are welcome.

## Contribute

If you think this could be better, please [open an issue](https://github.com/risadams/pride-flags/issues/new)!

Please note that all interactions in this organization fall under our [Code of Conduct](CODE_OF_CONDUCT.md).

## License

[MIT](LICENSE) © 1996+ Ris Adams
