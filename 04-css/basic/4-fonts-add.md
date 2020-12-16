# Подключение шрифтов

## @font-face

- Базовые начертания семейства **должны** иметь общее название `font-family`.
- Для каждого начертания **должны** быть указаны `font-weight` и `font-style`.
- В списке подключаемых форматов **должны** быть только WOFF2 и WOFF.
- Порядок подключения версий шрифта **должен** быть: WOFF2, WOFF.
- В форматах **может** не быть WOFF, если позволяет кроссбраузерность.
- В описании шрифта **должен** быть указан режим отрисовки `font-display`.

### Правильно

```css
@font-face {
  font-family: "PT Sans";
  font-weight: normal;
  font-style: normal;
  font-display: swap;
  src:
    url("../fonts/pt-sans-regular.woff2") format("woff2"),
    url("../fonts/pt-sans-regular.woff") format("woff");
}

@font-face {
  font-family: "PT Sans";
  font-weight: bold;
  font-style: normal;
  font-display: swap;
  src:
    url("../fonts/pt-sans-bold.woff2") format("woff2"),
    url("../fonts/pt-sans-bold.woff") format("woff");
}
```

### Неправильно

```css
@font-face {
  font-family: "PT Sans Regular";
  src:
    url("../fonts/pt-sans-regular.ttf") format("truetype"),
    url("../fonts/pt-sans-regular.woff") format("woff"),
    url("../fonts/pt-sans-regular.woff2") format("woff2");
}

@font-face {
  font-family: "PT Sans Bold";
  src:
    url("../fonts/pt-sans-bold.ttf") format("truetype"),
    url("../fonts/pt-sans-bold.woff") format("woff")
    url("../fonts/pt-sans-bold.woff2") format("woff2");
}
```

### Google Fonts

- Стили для шрифтов **должны** быть подключены с помощью `<link rel="stylesheet">` в `<head>`.
- В параметрах подключения **должны** быть только используемые семейства и начертания.
- В параметрах подключения должен быть указан режим отрисовки `display=swap`.
