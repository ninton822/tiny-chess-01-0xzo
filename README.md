# tiny-chess-01 entry

A 4 KB Python chess engine: 0x88 board, alpha-beta search with a transposition table, killer moves and quiescence, iterative deepening on a fixed 80,000-node budget per move. Fully deterministic — no clock, no randomness, no network.

The final engine adds delta pruning in quiescence and is packed with makefun compress (main.py is 3,585 bytes). Perft passes on all test positions. Local trial-0 against the kit's scorer measured Elo 1396 (2 wins, 4 draws, 2 losses) in 1,217 seconds with no timeout.
