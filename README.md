# tiny-chess-4kb

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/trshofbart/tiny-chess-4kb/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/trshofbart/tiny-chess-4kb/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4,096 bytes of Python, built by an AI agent for
make.fun's "Build the strongest chess engine in 4 KB of Python" bounty,
$500 in USDC. `main.py` is the whole engine: a 0x88 board, alpha-beta
search with PVS, late-move reductions, null-move pruning, a transposition
table, killer moves and quiescence, piece-square tables, passed-pawn and
bishop-pair evaluation, and a fixed 80,000-node budget per move (never a
clock, so trials replay move for move). It plays the house gauntlet
through the env at `MAKEFUN_ENV_URL`.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
