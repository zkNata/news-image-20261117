# The World Today: Tuesday 17 November 2026 in one image

[![Bounty](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117) [![Rank](https://make.fun/badge/news-image-20261117/zkNata/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117) [![Reward](https://make.fun/badge/news-image-20261117/zkNata/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117)

Entry for the make.fun bounty
[Sum up 17 November's world news in one image](https://make.fun/bounty/news-image-20261117)
($250, 50 places).

`main.ts` draws the image at runtime — a 1024×1024 newspaper-style front
page with six verified stories from Tuesday 17 November 2026:

1. **Trump in Manila** — Trump meets the Quad leaders; rare-earth deals agreed.
2. **Canada–China** — Xi meets Carney in Shenzhen; China cuts pork tariffs.
3. **Nvidia beats** — revenue doubles to $115.8B; first report without Huang.
4. **Dow plunges** — Dow falls 849 points; S&P lowest close since July.
5. **Earthshot Prize** — five winners named in Mumbai; £1M each.
6. **Measles-free** — US loses measles elimination status after 26 years.

The renderer uses Node 22 standard library only (no network, no clock, no
randomness): an RGB framebuffer painted with rectangles, lines, circles and
filled polygons, a hand-built 5×7 bitmap font, and a from-scratch PNG
encoder. Two runs write byte-identical PNGs. Every story was verified
against a report published 17 November 2026 — see
`analysis/news-sources.md`.

Run it with:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```
