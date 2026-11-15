# Manual test checklist: Colour Vocab page

Open `src/index.html` in a browser (see the README). Mark each item `Pass` or
`Fail` and note the date and browser.

Last run: 2026-11-16, built-in browser pane (Chromium), page served from a throwaway local static server on 127.0.0.1 (stopped afterwards) so that `style.css` and the images load. Items 1 to 3, 5 and 7 were read from the DOM; items 4 and 8 from the computed style, the resource list and the style sheets; item 6 at a 375 px wide emulated window.

| # | Check | Expected | Result |
| --- | --- | --- | --- |
| 1 | Exactly one `h1` | Text is "Colors" | Pass |
| 2 | Five colour titles (`h2.color-title`) | In order "Rojo", "Azul", "Anaranjado", "Verde", "Amarillo", each with font weight normal (400) | Pass |
| 3 | Five images | Each loads, has `alt` text `red`, `blue`, `orange`, `green`, `yellow` in that order, and is displayed 200 px wide and 200 px high | Pass |
| 4 | The stylesheet is applied | `style.css` is requested and loaded, and the title colours are `rgb(255, 0, 0)`, `rgb(0, 0, 255)`, `rgb(255, 165, 0)`, `rgb(0, 128, 0)` and `rgb(212, 169, 0)` | Pass |
| 5 | Page title | The tab shows "Spanish Vocabulary" | Pass |
| 6 | Narrow window (375 px wide) | The right edge of every image and every text line is at most 375 px, so nothing needs sideways scrolling | Pass |
| 7 | One extra heading | The `h2` "Learn the colors in Spanish!" comes before "Rojo" (six `h2` in all) | Pass |
| 8 | All styling is in the CSS | `index.html` has no `style` attribute and no `<style>` element | Pass |
