## UmePlus fonts

UmePlus fonts are modified Ume fonts for Japanese.

<http://www.geocities.jp/ep3797/modified_fonts_01.html>

I used these fonts for UmePlus fonts:

- Kanji = Ume fonts

  <https://osdn.net/projects/ume-font/releases/>

- Alphabet/Hiragana/Katakana, Full width alphabet = M+ fonts

  <https://osdn.net/projects/mplus-fonts/releases/>

Thanks to the authors.

### License

Ume fonts, M+ fonts: See docs-{ume,mplus}.

fontforge-scripts: Public Domain.

### Author

UTUMI Hirosi (utuhiro78 at yahoo dot co dot jp)

### How to update UmePlus fonts

1. Install fontforge

  ```
  $ sudo pacman -S fontforge
  ```

2. Extract files

  ```
  $ mkdir umeplus-tmp
  $ mv mplus-TESTFLIGHT-063.tar.xz umeplus-tmp/
  $ mv umefont_670.7z umeplus-tmp/
  $ mv umeplus-fonts-20180604.tar.xz umeplus-tmp/
  $ cd umeplus-tmp/
  $ tar xf umeplus-fonts-20180604.tar.xz
  $ mv umeplus-fonts-20180604 umeplus-fonts-dev
  $ mv umeplus-fonts-dev/update-umeplus.sh .
  ```

3. Update "update-umeplus-fonts.sh"

  ```
  $ leafpad update-umeplus-fonts.sh
  ```

  Change the lines:

  ```
  MPLUSVER="063"
  UMEVER="670"
  UMEPLUSVER="20180604"
  ```

4. Update UmePlus fonts

  ```
  $ ./update-umeplus.sh
  ```
