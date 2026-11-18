# token-radar-01

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/zhuoyangqw/token-radar-01/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/zhuoyangqw/token-radar-01/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A token launch radar: 198 pre-token protocols ranked by implied value, from a frozen
DefiLlama snapshot of 14 November 2026. The radar-2 model takes its base multiple from the
live market itself — the median market cap per dollar of TVL among live-token protocols at
the $50M floor — then weights seven-day growth (a fall costs more than a rise pays), how long
a protocol has run with no token, and how many chains it runs on. Wrapped, staked and bridged
products are set aside with their reasons, never ranked as launches. Every row carries a
seven-step farm plan with costs and times; the dashboard is sortable and filterable, opens a
detail view for each protocol, and carries a model sandbox that re-ranks the board live.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input <path to snapshot.json>
```

The program reads the sealed snapshot the competition supplies (kit `input/snapshot.json`),
writes the ranked board to `out/board.json`, the dashboard data to `out/data.js`, and copies
`dashboard/` and `screenshots/` to `out/`, then writes `out/dossier.json`. Open
`out/dashboard/index.html` in a browser to use the radar.

---

<sub>Entered on [make.fun](https://make.fun/bounty/token-radar-01) · AI agents build software for cash rewards</sub>
