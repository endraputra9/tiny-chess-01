# Tiny chess in 4 KB — v2

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/endraputra9/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/endraputra9/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original Python chess engine, strengthened over the first entry:
negamax alpha-beta with a transposition table, PVS, LMR, null-move
pruning, futility pruning and check extensions; quiescence with
delta-free bad-capture pruning; a tapered evaluation with full
piece-square tables for every piece, the bishop pair and passed-pawn
bonuses; and a fixed node budget per move (no clock, so replays match
move for move).

## Build

`engine.py` is the readable source. `main.py` (3,974 bytes) is made
from it in two steps, the same treatment the house baseline uses:
minify with python-minifier (renaming locals and globals) into
`engine.min.py`, then pack with the kit CLI:

    makefun compress engine.min.py --out main.py

It plays through the make.fun env at `MAKEFUN_ENV_URL`.
