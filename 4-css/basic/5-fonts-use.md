# Использование шрифтов

- Основное семейство шрифта **должно** быть указано на корневом элементе страницы.
- Начертания основного шрифта **должны** меняться с помощью `font-weight` и `font-style`.
- Дополнительные семейства **должны** применяться точечно, где они нужны.
- При указании шрифт **должен** дополняться семейством: `serif`, `sans-serif`, `monospace`.
- Свойство `font-weight` **должно** указываться единообразно: либо ключевыми словами, либо числовыми значениями.

## Правильно

```css
.page {
  font-family: "PT Sans", sans-serif;
}

.content h2 {
  font-family: "Futura", sans-serif;
  font-weight: bold;
}
```

## Неправильно

```css
.content {
  font-family: "PT Sans";
}

.content h2 {
  font-family: "Futura Bold";
}
```

## Неправильно

```css
.slogan {
  font-weight: bold;
}

h2 {
  font-weight: 700;
}
```
