# Префиксы

- В стилях **не должно** быть лишних префиксов, которые не нужны для браузерной совместимости.
- Префиксы **могут** использоваться для нестандартных свойств, значений и псевдоэлементов.
- Префиксы в селекторах **должны** быть продублированы с каждым вариантом префикса.
- Свойство без префикса **должно** идти после этого же свойства с префиксом.

## Правильно

```css
.button {
  border-radius: 5px;
}
```

## Неправильно

```css
.button {
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -o-border-radius: 5px;
  border-radius: 5px;
}
```

## Правильно

```css
.button::-moz-focus-inner {
  border: none;
}

.question__title::-webkit-details-marker {
  display: none;
}
```

## Правильно

```css
.block::-moz-selection {
  color: #ff0000;
}

.block::selection {
  color: #ff0000;
}
```

## Неправильно

```css
.block::-moz-selection,
.block::selection {
  color: #ff0000;
}
```

## Правильно

```css
.select__control {
  -webkit-appearance: none;
  appearance: none;
}
```

## Неправильно

```css
.select__control {
  appearance: none;
  -webkit-appearance: none;
}
```
