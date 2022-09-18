# Klingon Fonts

## Source

| **Directory** | pIqaD      | pIqaD bitmap   |
|:--------------|:-----------|:---------------|
| **Name**      | [CODE2000] | [Unifont CSUR] |
| **Version**   | v1.175     | v15.0.01       |
| **Updated**   | 2022-09-15 | 2022-09-13     |

[CODE2000]: https://code2001.com/code2000_page.htm
[Unifont CSUR]: https://unifoundry.com/unifont/index.html

## Build

```Bash
# pIqaD
svgicons2svgfont -w -c -y -a --fontname=pIqaD -o pIqaD.svg pIqaD/*.svg
svg2ttf pIqaD.svg pIqaD.ttf
ttf2eot pIqaD.ttf pIqaD.eot
ttf2woff pIqaD.ttf pIqaD.woff
cat pIqaD.ttf | ttf2woff2 > pIqaD.woff2

# pIqaD bitmap
svgicons2svgfont -w -c -y -a --fontname=pIqaD -o pIqaD-bitmap.svg pIqaD-bitmap/*.svg
svg2ttf pIqaD-bitmap.svg pIqaD-bitmap.ttf
ttf2eot pIqaD-bitmap.ttf pIqaD-bitmap.eot
ttf2woff pIqaD-bitmap.ttf pIqaD-bitmap.woff
cat pIqaD-bitmap.ttf | ttf2woff2 > pIqaD-bitmap.woff2
```

See [svgicons2svgfont], [svg2ttf], [ttf2eot], [ttf2woff], [ttf2woff2].

[svgicons2svgfont]: https://github.com/nfroidure/svgicons2svgfont
[svg2ttf]: https://github.com/fontello/svg2ttf
[ttf2eot]: https://github.com/fontello/ttf2eot
[ttf2woff]: https://github.com/fontello/ttf2woff
[ttf2woff2]: https://github.com/nfroidure/ttf2woff2
