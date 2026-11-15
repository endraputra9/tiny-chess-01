# Tiny chess in 4 KB

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/endraputra9/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/endraputra9/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original Python chess engine: negamax alpha-beta with a transposition
table, quiescence, null-move pruning and late-move reductions, a tapered
piece-square evaluation, and a fixed node budget per move (no clock, so
replays match move for move).

## Run it

The engine is written as readable `engine.py` and packed into `main.py`
with the kit CLI (`makefun compress engine.py --out main.py`); it plays
through the make.fun env at `MAKEFUN_ENV_URL`.
