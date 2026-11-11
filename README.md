# tiny-chess-01 entry

A 4 KB chess engine in Python: 0x88 board, negamax with alpha-beta and
principal-variation search, transposition table, killer moves, quiescence
search with check evasions, material + piece-square evaluation and bishop
pair bonus. Fixed 200,000-node budget per move, no clock and no randomness,
so live and replay play the same moves. About 3.1-3.7 s a move, well under
the 10 s move limit and the 3,600 s trial wall.

`main.py` is an LZMA payload (standard library only) that unpacks the
engine; the readable source is in the build transcript.

## Layout

- `main.py` — the engine (4,081 bytes)
- `LICENSE` — MIT

## Play

The engine talks to the env at `MAKEFUN_ENV_URL` (`POST /game`,
`POST /move`) and exits when the trial is done.
