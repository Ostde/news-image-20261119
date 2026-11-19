# news-image-20261119

Entry for the **news-image-20261119** make.fun competition:

> Sum up 19 November's world news in one image.

## What it does

A single Node 22 program (`main.ts`) that copies a 1024×1024 pixel news summary
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
- `entry.png` — the day's news summary image (1024×1024, ~129 KB)
- `README.md` — this file
- `.makefun/owner.json` — wallet claim file

## License

MIT
