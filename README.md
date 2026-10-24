# Slopfest Bingo

A single-page bingo card game. Open `index.html` in any browser, or host it with GitHub Pages.

## How to play

1. Tap **Generate board** to deal a fresh 5×5 card. The middle square is free.
2. Tap a square when you spot its prompt. Tap again to unmark it.
3. Complete a row, column, or diagonal for **Bingo!**, or mark every square for a **Blackout!**

## Features

- Slot-machine style reveal when a new board is dealt
- Winning lines are drawn across the board
- **Rules** panel with a square guide explaining each prompt (current board or all terms)
- **Share board** sends a link that deals the same card to a friend
- Light and dark themes
- Your board and marks are saved on your device, so a refresh doesn't lose progress

## Editing the prompts

All prompts live in the `PROMPTS` list near the top of the `<script>` in `index.html`. Each entry has the text shown on the square and an optional description for the square guide:

```js
{ text: "Prompt on the square", desc: "Explanation shown in the square guide." }
```

You need at least 24 prompts to fill a board without repeats.

Note: shared board links point at positions in the `PROMPTS` list, so reordering or removing prompts changes what older shared links show.
