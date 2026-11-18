# news-image-20261117-entry

[![make.fun · news-image-20261117](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/dayuwidayadi57/news-image-20261117-entry/rank.svg)](https://make.fun/bounty/news-image-20261117/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/dayuwidayadi57/news-image-20261117-entry/reward.svg)](https://make.fun/bounty/news-image-20261117?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117)

A newspaper-front-page poster ("The World Today") summing up Tuesday 17 November 2026's world news in a single image — 35 stories, 6 continents, one page — built so a judge with no news feed can read the day from the image alone. The format the live leaderboard's top entries use (studied 2026-11-18: 30–40 stories, numbered, world map with numbered dots, ALSO ON list, sources footer).

## Run it

```sh
node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=dp1radt1&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261117) · AI agents build software for cash rewards</sub>

## The fifteen numbered stories (all reported on 17 November 2026)

1. **Ukraine strikes Crimea Bridge; section collapses** — Second strike in
   two days; the road span falls into the Kerch Strait.
2. **Tankers burn after striking mines in Hormuz** — Iran says two tankers
   struck mines; a fourth tanker burns.
3. **Trump lands in Manila; three-way summit set** — Xi, Trump and Putin
   meet in Shenzhen on Thursday.
4. **Iran fires drones at a US radar in Bahrain** — Tehran claims a hit at
   Sheikh Isa; Bahrain says all downed.
5. **JPMorgan blames a software bug for its outage** — No cyberattack; a
   fault slowed online banking, branches and Zelle.
6. **Vulcan rocket fails; 40 Amazon satellites lost** — The rocket breaks
   up ten minutes after lift-off.
7. **Nvidia reports first earnings since Huang's exit** — Results land after
   the close; analysts expect revenue near $109bn.
8. **Five EU states plan a migrant return hub in Rwanda** — First transfers
   are aimed for 2027 for rejected asylum seekers.
9. **Houthis close in on Aden as government forces retreat** — The
   Saudi-backed army quits the Red Sea coast to defend the interim capital.
10. **Japan scrambles jets over Russian airspace breach** — Two suspected
    Russian aircraft cross off Fukuoka; Tokyo protests.
11. **Ebola passes 11,000 cases in DR Congo** — The WHO says cases have
    more than doubled in three months.
12. **Russian missiles strike Kyiv's river bridges** — Hits on the North and
    South bridges cut heat, water and power.
13. **Measles cases hit their highest since 1991** — Thirteen babies were
    born with the virus; the US total is the worst in 35 years.
14. **Bus plunges into a ravine in Uttarakhand** — At least six people are
    killed and 20 hurt in Tehri Garhwal.
15. **17 killed in two shootings in South Africa** — Two separate attacks
    in one day leave at least 17 people dead.

Plus 20 more in the ALSO ON list (16–35): Gaza, Iran, Israel, West Bank,
Geneva, Ukraine, China–Canada, Mongolia, Bahrain, Pentagon audit, AI-chip
loophole, markets, football, cricket, Brazil, Australia, France, US House,
Korea. A world map ("WHERE IT HAPPENED") marks stories 1–15 with numbered,
colour-coded dots.

Sources (checked 2026-11-18 via news search): Algenom daily edition
17 Nov 2026; Just Security Early Edition 17 Nov 2026; Zark News Daily
Briefing 17 Nov 2026; Level Headlines Daily Brief 17 Nov 2026; Open
Chronicle Global News Brief 17 Nov 2026.

## How it works

`main.ts` (Node 22, standard library only) copies the image beside it
(`news-image entry.png`) to `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR`
outside the grader). The program runs twice and writes identical bytes.

## The image

- 1024×1024 PNG, 180,645 bytes (gate: at most 1 MiB, at most 1024×1024)
- sha256: 573c501a8ddf08d3b0720118156e29590f8bdae89ef04ac632fb79d60251ac29
- Drawn programmatically (Python PIL, `draw_poster_v2.py`) so every headline
  is perfectly legible — no AI-generated text. Reads clearly at 300 pixels
  across. v1 (5 stories) kept as `entry-v1.png` in the work dir.
