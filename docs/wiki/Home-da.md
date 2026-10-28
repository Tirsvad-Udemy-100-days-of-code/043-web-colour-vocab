[English](Home) · **Dansk** · [Bahasa Malaysia](Home-ms)

# Colour Vocab

En flashcard-side til at lære farverne på spansk, lavet kun med HTML og CSS.

![Den færdige side](images/colour-vocab.png)

## Gloser

| Spansk | English | Dansk | Bahasa Malaysia |
| --- | --- | --- | --- |
| Rojo | red | rød | merah |
| Azul | blue | blå | biru |
| Anaranjado | orange | orange | oren |
| Verde | green | grøn | hijau |
| Amarillo | yellow | gul | kuning |

## Sådan kører du den

Åbn `src/index.html` i en vilkårlig browser. Der er intet at installere.

## Sådan virker den

`index.html` linker til et eksternt stylesheet, `style.css`. Opgavens regel er,
at alle ændringer sker i CSS og ingen i HTML.

1. **Link stylesheetet.** `<link rel="stylesheet" href="./style.css" />`.
   Test linket ved midlertidigt at sætte `body { background-color: pink; }` og
   se, at siden ændrer sig.
2. **Farv hver titel efter dens betydning.** Hver titel har et `id` (`red`,
   `blue`, `orange`, `green`, `yellow`), så `#red { color: red; }` rammer kun
   *Rojo*. `id`'et er et hint, hvis du ikke kender det spanske ord.
3. **Gør titlerne normale i vægt.** Alle titler har klassen `color-title`, så
   én regel dækker dem: `.color-title { font-weight: normal; }`.
4. **Størrelse på billederne.** `img { height: 200px; width: 200px; }` gør alle
   farvefelter lige store.

Se et preview efter hvert trin, så en fejl opdages, mens den er lille.

### Bemærkning om gul

Almindelig `yellow` er svær at læse på hvid baggrund, så *Amarillo* bruger
`#d4a900`.

## Skærmbillede

Skærmbilledet er taget med headless Chrome i et 480 px bredt vindue:

```bash
chrome --headless=new --hide-scrollbars --window-size=480,1490 \
  --screenshot=docs/wiki/images/colour-vocab.png file:///sti/til/src/index.html
```
