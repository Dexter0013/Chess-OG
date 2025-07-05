<p align="center"> <h1 align="center">♟️ Pygame Chess/ Chess-OG</h1> <p align="center">A 2-player chess game built using Python and Pygame</p> </p>

<p align="center"> <img src="https://img.shields.io/badge/python-3.9%2B-blue?style=flat-square" /> <img src="https://img.shields.io/badge/Pygame-2.1.0-green?style=flat-square" /> <img src="https://img.shields.io/badge/Chess-Classic-black?style=flat-square" /> <img src="https://img.shields.io/badge/UI-Grid%20Board-brown?style=flat-square" /> <img src="https://img.shields.io/badge/GameMode-Two%20Player-lightgrey?style=flat-square" /> </p>
🎮 Overview
A fully playable chess game built with Pygame. Features include:

<details> <summary><strong>🧩 Dynamic Board Rendering</strong></summary>

The 8×8 board is drawn with alternating light and dark squares. Each square is scaled based on the window size using WIDTH // 8.

</details>

<details> <summary><strong>🖼️ Image-Based Chess Pieces</strong></summary>

Pieces are loaded from PNG assets and scaled to fit each square. Each type (pawn, knight, queen, etc.) is rendered in full color with distinct images for white and black.

</details>

<details> <summary><strong>🔄 Turn-Based Gameplay</strong></summary>

Players take alternate turns starting with white. The current player is tracked and toggled after each valid move.

</details>

<details> <summary><strong>✅ Basic Movement Validation</strong></summary>

Each piece’s movement is validated based on classical chess rules. The game prevents illegal moves and captures pieces of the opposite color.

</details>

<details> <summary><strong>♟️ Pawn Promotion</strong></summary>

When a pawn reaches the final rank, it is automatically promoted to a queen of the same color.

</details>

<details> <summary><strong>⛔ Checkmate and Stalemate Detection</strong></summary>

After every move, the game checks if the current player has no valid moves and is in check. If true, a checkmate message is printed. If not in check but still without moves, it's a stalemate.</details>
🧩 How It Works
<details> <summary><strong>🕹️ Board and Pieces</strong></summary>

8x8 grid rendered dynamically using alternating colors

Each square sized automatically (WIDTH // 8)

Pieces loaded from PNG files and scaled to fit squares

</details>

<details> <summary><strong>🎯 Gameplay Mechanics</strong></summary>

Turn-based: Alternates between white and black

Piece selection: Click to select, then click valid destination

Highlighting: Selected piece's square is highlighted in yellow

Promotion: Pawns automatically convert to queens upon reaching last rank

End conditions: Checkmate and stalemate detected and printed

</details>

<details> <summary><strong>🤖 Movement Logic</strong></summary>

Supports standard chess movements:

Pawn: forward moves, double move, diagonal capture

Rook: vertical & horizontal movement

Knight: L-shape jumps

Bishop: diagonal movement

Queen: combined rook + bishop moves

King: 1-square in any direction

</details>

<details> <summary><strong>⚠️ Game Over Detection</strong></summary>

is_check: detects if a king is under attack

is_game_over: verifies if current player has any legal moves

Console prints "Checkmate! <Player> loses." or "Stalemate!"

</details>

<summary><strong>📦 Folder Layout</strong></summary>

```text
chess_game/
│
├── images/               # Contains all PNG assets for chess pieces
│   ├── black_pawn.png
│   ├── white_queen.png
│   └── ...etc
│
├── main.py               # Main game script
├── README.md             # You're reading this!
