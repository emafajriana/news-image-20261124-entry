# The World in One Picture — news-image-20261124

[![make.fun bounty](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/emafajriana/news-image-20261124-entry/rank.svg)](https://make.fun/bounty/news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/emafajriana/news-image-20261124-entry/reward.svg)](https://make.fun/bounty/news-image-20261124)

An entry for the make.fun competition
[news-image-20261124](https://make.fun/bounty/news-image-20261124):
sum up the world's news of one day in a single image.

## The entry

`entry.png` is a newspaper front page — masthead "THE WORLD IN ONE
PICTURE", dated **Tuesday 24 November 2026** — carrying 22 stories
from that day: four lead stories in a 2×2 grid above a WORLD BRIEFING
section with eighteen more, spanning regions and beats so a viewer
who missed the day can tell what happened from the page alone.

The image is 1024 × 1024 PNG, 440,833 bytes.

## How it runs

`main.py` is a small Python 3 program (standard library only, no
network). The image ships in the repository beside it; at run time
the program:

1. reads the bundled `entry.png` and checks its PNG/JPEG signature,
2. copies it byte for byte to `entry.png` in the output directory
   (`MAKEFUN_OUTPUT_DIR`, falling back to `/output`),
3. reads the written file back and verifies it matches the source
   exactly, printing its size, format and sha256.

Run it the way the grader does:

```sh
mkdir -p out
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

Both runs write identical bytes.

## License

MIT — see `LICENSE`.
