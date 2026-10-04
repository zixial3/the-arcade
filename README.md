# The Arcade

A minimal static site for CS 5610 with a 5×5 mini crossword built in HTML and CSS only.

**Live site:** _add the GitHub Pages URL here_

## Structure

```
index.html, home.css     landing page
game/                    crossword + game.css
about/                   about page + about.css
contact/                 contact page + contact.css
styles/global.css        shared tokens, layout, navbar
assets/                  SVG preview image and favicon
```

## Crossword, without JavaScript

- Grid: CSS Grid, `repeat(5, 1fr)`, square cells via `aspect-ratio`.
- Cells: `<input maxlength="1">` with an `aria-label` and `aria-describedby` to its clues.
- Check: each input's `pattern` is its answer; a checkbox + `:has()` / `:valid` / `:invalid` marks squares.
- Reveal: `<details>` / `<summary>`; answers appear in the grid.
- Clear: `<button type="reset">`.

Font: [Source Serif 4](https://fonts.google.com/specimen/Source+Serif+4) via Google Fonts.
