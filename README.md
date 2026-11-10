# Four in a Row

**A Connect 4 game for kids. Made for Manav.**

Play it online: **https://theonekik.github.io/connect4-kids/**

No ads. No tracking. No accounts. One HTML file, no dependencies, works offline.

---

## What it is

A classic drop-the-counter game on a 7 by 6 board. Line up four of your colour in a
row, column or diagonal. First to four wins the round.

You can play against another person on the same screen, or against the computer.

## How to play

- **Click or tap** any column to drop your counter.
- The ghost counter shows where it will land.
- **Arrow keys** move between columns, **Enter** or **Space** drops.
- **Undo** takes back your last move. Against the computer it takes back both moves,
  so you get your turn back.
- **New game** clears the board. The score keeps counting until you reload.

## The computer opponent

It is built to be beatable by a child. It takes a win when one is available and blocks
your four most of the time, but not always. No lookahead search, no perfect play.

## Accessibility

- Full keyboard play with visible focus rings.
- Screen readers announce turns and results through a live region.
- Respects `prefers-reduced-motion`: the drop animation is skipped, the game stays playable.
- Colour is never the only signal. The winning four get a white ring and a pulse, and the
  turn label names the colour in text.

## Testing

The file carries its own logic tests. Open `index.html?test=1` and the result appears on
the root element as `data-tests`:

```
data-tests="pass:10/10"
data-failures="none"
```

It covers horizontal, vertical and both diagonal wins, that three in a row is not a win,
gravity, a full column being unplayable, a full board counting as a draw, and the
computer spotting an immediate win.

## Running locally

Open `index.html` in any browser. There is no build step.

## Licence

MIT. See [LICENSE](LICENSE).
