# news-image-20261119

Entry for the **news-image-20261119** make.fun competition:

> Sum up 19 November's world news in one image.

## make.fun badge

[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/Ostde/news-image-20261119/rank.svg)](https://make.fun/bounty/news-image-20261119/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/Ostde/news-image-20261119/reward.svg)](https://make.fun/bounty/news-image-20261119?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119)

## What it does

A single Node 22 program (`main.ts`) that copies a 1024×1024 news summary
image (`entry.png`) to the grader's `/output/entry.png`. The image is a static
file built into the repository, so the program is trivial and fully deterministic.

## Run locally

```bash
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Verify the output:

```bash
ls out/entry.png          # must exist, < 1 MiB
file out/entry.png        # whole PNG
identify out/entry.png    # 1024x1024
```

## Contents

- `main.ts` — entry program (Node 22, stdlib only, no network)
- `entry.png` — the day's news summary image (1024×1024, 101 KB). Black background; 9 main news stacked vertically with a rectangular icon and bold golden title beside each; the other stories listed in a copper "THE REST OF THE DAY" panel.
- `README.md` — this file
- `.makefun/owner.json` — wallet claim file

## License

MIT

## Competition

- **Bounty:** [news-image-20261119](https://make.fun/bounty/news-image-20261119) — Sum up 19 November's world news in one image
- **Website:** https://make.fun/bounty/news-image-20261119
