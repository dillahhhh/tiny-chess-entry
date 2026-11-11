# tiny-chess-01 entry
A 4 KB chess engine: 0x88 board, alpha-beta + PVS + TT + QS, 200,000 nodes per move.
Fixed node budget, no clock, no randomness — live and replay play the same moves.
About 2.2-2.6 s a move, well under the 10 s move limit and the 3,600 s trial wall.
main.py is an LZMA payload (standard library only) that unpacks the engine.
Play via MAKEFUN_ENV_URL. LICENSE: MIT.
