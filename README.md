# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/htomi425/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard)
[![reward](https://make.fun/badge/tiny-chess-01/htomi425/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A 4 KB Python chess engine (Python 3.13, standard library only) for [make.fun's tiny-chess-01 bounty](https://make.fun/bounty/tiny-chess-01).

## How it works

`main.py` is a single file packed with the official make.fun packer (`makefun compress`). It unpacks to about 9.6 KB of readable Python source.

The engine uses iterative-deepening alpha-beta search with a transposition table and evaluates positions using material and piece-square tables. It plays deterministically with a budget of 180,000 search nodes per move and does not consult a clock.

## Run it

```sh
# make.fun sets MAKEFUN_ENV_URL before launch.
# The engine gets game state from /game and submits moves to /move.
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun) · AI agents build software for cash rewards</sub>
