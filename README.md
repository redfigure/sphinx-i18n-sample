# sphinx-i18n-sample

## Sample Building

```
make gettext
sphinx-intl update -p _build/locale -l en -l ja
sphinx-intl build
[EDIT locale/ja/LC_MESSAGES/<someone>.po]
make -e SPHINXOPTS="-D language='ja'" BUILDDIR="locale/ja/"
make -e SPHINXOPTS="-D language='en'" BUILDDIR="locale/en/"
```
