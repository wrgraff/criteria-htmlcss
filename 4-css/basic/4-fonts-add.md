# Подключение шрифтов

## @font-face

- Базовые начертания семейства **должны** иметь общее название `font-family`.
- Для каждого начертания **должны** быть указаны `font-weight` и `font-style`.
- В описании шрифта **должен** быть указан режим отрисовки `font-display`.

### Правильно

```css
@font-face {
  font-family: "PT Sans";
  font-weight: normal;
  font-style: normal;
  font-display: swap;
  src: url("../fonts/pt-sans-regular.woff2") format("woff2");
}

@font-face {
  font-family: "PT Sans";
  font-weight: bold;
  font-style: normal;
  font-display: optional;
  src: url("../fonts/pt-sans-bold.woff2") format("woff2");
}
```

### Неправильно

```css
@font-face {
  font-family: "PT Sans Regular";
}

@font-face {
  font-family: "PT Sans Bold";
}
```
