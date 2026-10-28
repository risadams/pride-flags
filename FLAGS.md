# Flag references

Every flag in `src/pride-flags.scss` should match a published design. This file records where each flag's colors came from, so a flag can be re-checked or corrected.

**Sources**

- **prideflags.org**: the primary reference. Each flag has an SVG at `https://www.prideflags.org/static/search/data/img/<name>.svg` with exact colors and stripe layout.
- **Wikimedia Commons**: used for flags prideflags.org does not list. Community uploads that sometimes disagree with each other.
- **LGBTQIA+ Wiki [Pride flag gallery](https://lgbtqia.fandom.com/wiki/Pride_flag_gallery)**: gives stripe counts and shapes only, with no color values. Used to check layout.

Each was checked on 2026-10-28. Every flag in the "Verified" tables was also compared visually, side by side with its reference SVG, in headless Chrome.

## Verified against prideflags.org

| Flag | Reference file | Notes |
| --- | --- | --- |
| `agender` | agender_pride_flag | |
| `aromantic`, `aromantic-spectrum` | aromantic_pride_flag | Same flag. `aromantic-spectrum` is an alias. |
| `asexual` | asexual_pride_flag | |
| `bear-brotherhood` | bear_pride_flag | Stripes only. The reference has a black paw print in the top left that is not drawn. |
| `bigender` | bigender_pride_flag_7_stripe | |
| `bisexual` | bisexual_pride_flag | Bands are 2:1:2. |
| `bxy` | bxy_pride_flag | New. |
| `demiboy`, `demigirl` | demiboy_pride_flag, demigirl_pride_flag | |
| `demiromantic`, `demisexual` | demiromantic_pride_flag, demisexual_pride_flag | Triangle and stripe geometry were corrected. |
| `gendercreative` | gendercreative_pride_flag | New. |
| `genderfluid` | genderfluid_pride_flag | |
| `genderflux` | genderflux_pride_flag | Colors were wrong before. |
| `genderqueer` | genderqueer_pride_flag | |
| `gxrl` | gxrl_pride_flag | New. |
| `intersex` | intersex_pride_flag | Ring size was corrected. |
| `labrys` | lesbian_pride_flag_labrys | Background color corrected. |
| `lipstick-lesbian` | lipstick_lesbian_pride_flag_without_kiss | New. The "with kiss" variant is not drawn. |
| `littlefluid` | littlefluid_pride_flag | New. |
| `neutrois` | neutrois_pride_flag | |
| `nonbinary` | nonbinary_pride_flag | The bottom stripe is black, not dark gray. |
| `nxnbinary` | nxnbinary_pride_flag | New. This is the yellow version. |
| `pangender` | pangender_pride_flag_white_center | Seven mirrored bands. It was eight bands before. |
| `pansexual` | pansexual_pride_flag | |
| `polysexual` | polysexual_pride_flag | |
| `progress` | progress_pride_flag | Uses that file's rainbow (`#ee2824 ...`), which differs from `traditional`. |
| `philadelphia` | gay_pride_flag_philadelphia | |
| `traditional` | gay_pride_1979 | |
| `transgender` | transgender_pride_flag | |

`intersex-inclusive` and `new-pride` reuse the chevron colors from `progress`. `intersex-inclusive` shares the intersex ring color.

## Verified against Wikimedia Commons

| Flag | Commons file | Notes |
| --- | --- | --- |
| `abrosexual` | Abrosexual flag.svg | |
| `graysexual` | Grey asexuality flag.svg | |
| `omnisexual` | Omnisexual Pride-Flag.svg | |
| `gilbert-baker`, `pride-1978` | Gay flag 8.svg | `pride-1978` is the same palette without hot pink. |
| `polyamorous-new` | Tricolor Polyamory Pride Flag.svg | Red Howell's 2022 design. Geometry is approximated with gradients and compared visually. |

## Checked for layout only (Fandom gallery)

The gallery's stripe counts agree with our flags for `androgyne` (3), `neutrois` (3), `twink` (3), `genderflux` (6), `gay-men` (7), `lesbian` (7), `demigender` (7) and `bear-brotherhood` (7). Colors for these are still unverified unless listed above.

## Unverified or suspect

| Flag | Problem |
| --- | --- |
| `asexual-spectrum` | The gallery lists the asexual spectrum flag with 4 stripes. Ours has 5 and matches the gray-asexual design (see `graysexual`). Probably wrong. |
| `unlabeled` | The gallery lists it with 4 stripes. Ours has 5. Probably wrong. |
| `sapphic` | The gallery lists the sapphic flag with 3 stripes and a violet flower. Ours has 4 stripes, which looks like the "Lesbian (Sappho)" flag. Name or design needs checking. |
| `queer` | The gallery lists queer under 8+ stripes and also as a chevron flag. Ours is a diagonal design. |
| `androgyne` | Layout matches the gallery (3 stripes). Colors are from memory. |
| `lesbian` | Seven-stripe sunset flag. Layout matches the gallery. Colors are from memory. |
| `gay-men`, `trans-inclusive`, `demigender` | Colors from memory. `demigender` stripe layout matches the gallery. |
| `hijra`, `metagender` | Not in any of the references. Unchanged from earlier versions. |
| `intersex-inclusive`, `new-pride`, `social-justice` | Chevron and triangle geometry unchanged. `new-pride` looks different from the published design. |
| `polyamory` | Blue, red, black and a yellow π. Colors are CSS names. |
| `ally-pride`, `pink-triangle` | Unchanged. Not in any of the references. |
| `pride-of-africa`, `puppy`, `leather`, `rubber`, `drag`, `twink` | Complex shapes, unchanged. Not in any of the references. |

## Listed by the references but not added

- **Needs artwork we haven't drawn:** `doe`, `pocket-gender`, `ingender`, the UK gay flag, and the "with kiss" lipstick lesbian flag.
- **Variants of flags we already have:** the other agender and nonbinary variants, the `pangender` yellow-center flag, the rainbow lesbian flag, the transgender variants, `trans-intersex`, and the two Trans PoC "new pride" flags.
- **Fandom flags with no color source:** the gallery lists many more flags, such as maverique, achillean and aegosexual. It has no color values, so none were added.
