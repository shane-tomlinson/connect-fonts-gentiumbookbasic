# connect-fonts-gentiumbookbasic

Gentium Book Basic fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-gentiumbookbasic");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/genbkbasb/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/genbkbasb,genbkbasbi,genbkbasi,genbkbasr/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* genbkbasb
* genbkbasbi
* genbkbasi
* genbkbasr-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/genbkbasb/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin

5. Set your CSS up to use the new font by using the "Gentium Book Basic" font-family.
```
    body {
      font-family: 'Gentium Book Basic', 'sans-serif', 'serif';
    }
```

## Font Info
Gentium Book Basic

The Gentium Book Basic font family is based on the original Gentium design, but with additional weights. The family comes with a complete regular, bold, italic and bold italic set of fonts. The supported character set, however, is much smaller than for the main Gentium Plus fonts. These "Basic" fonts support only the Basic Latin and Latin-1 Supplement Unicode ranges, plus a selection of the more commonly used extended Latin characters, with miscellaneous diacritical marks, symbols and punctuation. In particular, these fonts do not support full extended Latin IPA, complete support for Central European languages, Greek and Cyrillic. The "Gentium Basic" family is very similar but has a slightly lighter weight.

* Copyright: Copyright (c) SIL International, 2003-2008.
* Trademark: Gentium is a trademark of SIL International.
* Designer: J. Victor Gaultney and Annie Olsen
* Designer URL: http://www.sil.org/~gaultney
* Vendor: SIL International
* Vendor URL: http://scripts.sil.org/

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-gentiumbookbasic
* Repo: https://github.com/shane-tomlinson/connect-fonts-gentiumbookbasic.git
* Bugs: https://github.com/shane-tomlinson/connect-fonts-gentiumbookbasic/issues

## Font pack Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 1.1 of the SIL Open Font License

  http://scripts.sil.org/OFL

