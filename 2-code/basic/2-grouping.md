# Группировка файлов

Файлы схожих типов **должны** быть сгруппированы в папки: картинки, стили, скрипты, шрифты. Если внутри папок файлов становится много или выделяются подгруппы, **можно** добавить вложенные папки.

## Правильно

```
images/
  logo.svg
  icons/
    32x32.png
    16x16.png
scripts/
  menu.js
  map.js
styles/
  blocks/
    header.css
    footer.css
  index.css
  fonts.css
index.html
```

## Неправильно

```
assets/
  logo.svg
  icon-32x32.png
  icon-16x16.png
  menu.js
  map.js
  header.css
  footer.css
  index.css
  fonts.css
index.html
```
