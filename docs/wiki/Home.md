**English** · [Dansk](Home-da) · [Bahasa Malaysia](Home-ms)

# Colour Vocab

A one-page flashcard site for learning the colours in Spanish, built with HTML
and CSS only.

![The finished page](images/colour-vocab.png)

## Vocabulary

| Spanish | English | Dansk | Bahasa Malaysia |
| --- | --- | --- | --- |
| Rojo | red | rød | merah |
| Azul | blue | blå | biru |
| Anaranjado | orange | orange | oren |
| Verde | green | grøn | hijau |
| Amarillo | yellow | gul | kuning |

## How to run

Open `src/index.html` in any browser. There is nothing to install.

## How it works

`index.html` links an external stylesheet, `style.css`. The exercise rule is
that all changes are made in the CSS and none in the HTML.

1. **Link the stylesheet.** `<link rel="stylesheet" href="./style.css" />`.
   To test the link, temporarily set `body { background-color: pink; }` and
   check that the page changes.
2. **Colour each title by its meaning.** Every title has an `id` (`red`,
   `blue`, `orange`, `green`, `yellow`), so `#red { color: red; }` styles only
   *Rojo*. The `id` is a hint if you do not know the Spanish word.
3. **Make the titles normal weight.** All titles share the class
   `color-title`, so one rule covers them: `.color-title { font-weight: normal; }`.
4. **Size the images.** `img { height: 200px; width: 200px; }` makes every
   swatch the same size.

Preview after each step so a mistake is caught while it is still small.

### Note on yellow

Plain `yellow` is hard to read on a white page, so *Amarillo* uses `#d4a900`.

## Screenshot

The screenshot was taken with headless Chrome at a 480 px wide window:

```bash
chrome --headless=new --hide-scrollbars --window-size=480,1490 \
  --screenshot=docs/wiki/images/colour-vocab.png file:///path/to/src/index.html
```
