# NOTE

This has been forked from the original repo because I need the rotated font to have "Rotated" suffix as its font name to be able to use [this KOReader patch](https://gist.github.com/starryalley/8501e0218d25c49b9c1aa537399b4185). 

Unfortunately it looks like [KOReader](https://koreader.rocks/) uses many rules to determine the "font name" of a font. It can be family name, or can be "Preferred Family Name" in TTF Names (as seen in fontforge). Simply renaming "fontname" and "fullname" is not enough. That's why I made this small change.

It's an awesome work from the original author. I've been enjoying this to read many Traditional Chinese books in vertical layout in [KOReader](https://koreader.rocks/).

# tategakifont

縦書きの対応がないシステムで縦書きがほしい時にフォントを９０度回して画面も９０度回したら縦書きだ。

このスクリプトはフォントを正確に９０度で回してくれる。

If you need vertical text in a syntem that does not support it, you can rotate by 90 degrees the font and the screen instead.

You can use this script to rotate the font by 90 degrees correctly.

## rules for rotation

The rules for rotating the glyphs can be found [here](https://www.unicode.org/reports/tr50/)

## Usage

You need python and fontforge installed.
You might also need to install some of the dependencies listed as imports at the top of `main.py` using `pip` or some other package manager.
To use the script, in the command line write: `python main.py input output`, where "input" is the input file name and "output" the output file name.

