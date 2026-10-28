[English](Home) · [Dansk](Home-da) · **Bahasa Malaysia**

# Colour Vocab

Laman kad imbas satu halaman untuk belajar warna dalam bahasa Sepanyol,
dibina dengan HTML dan CSS sahaja.

![Halaman siap](images/colour-vocab.png)

## Kosa kata

| Sepanyol | English | Dansk | Bahasa Malaysia |
| --- | --- | --- | --- |
| Rojo | red | rød | merah |
| Azul | blue | blå | biru |
| Anaranjado | orange | orange | oren |
| Verde | green | grøn | hijau |
| Amarillo | yellow | gul | kuning |

## Cara menjalankan

Buka `src/index.html` dalam mana-mana pelayar. Tiada apa-apa untuk dipasang.

## Cara ia berfungsi

`index.html` memaut helaian gaya luaran, `style.css`. Peraturan latihan ini
ialah semua perubahan dibuat dalam CSS dan tiada dalam HTML.

1. **Pautkan helaian gaya.** `<link rel="stylesheet" href="./style.css" />`.
   Untuk menguji pautan, tetapkan sementara `body { background-color: pink; }`
   dan semak bahawa halaman berubah.
2. **Warnakan setiap tajuk mengikut maksudnya.** Setiap tajuk mempunyai `id`
   (`red`, `blue`, `orange`, `green`, `yellow`), jadi `#red { color: red; }`
   hanya menggayakan *Rojo*. `id` ialah petunjuk jika anda tidak tahu
   perkataan Sepanyolnya.
3. **Jadikan tajuk berat biasa.** Semua tajuk berkongsi kelas `color-title`,
   jadi satu peraturan meliputi semuanya: `.color-title { font-weight: normal; }`.
4. **Saiz imej.** `img { height: 200px; width: 200px; }` menjadikan setiap
   petak warna sama saiz.

Pratonton selepas setiap langkah supaya kesilapan dikesan semasa masih kecil.

### Nota tentang kuning

`yellow` biasa sukar dibaca pada latar putih, jadi *Amarillo* menggunakan
`#d4a900`.

## Tangkapan skrin

Tangkapan skrin diambil dengan Chrome headless dalam tetingkap lebar 480 px:

```bash
chrome --headless=new --hide-scrollbars --window-size=480,1490 \
  --screenshot=docs/wiki/images/colour-vocab.png file:///laluan/ke/src/index.html
```
