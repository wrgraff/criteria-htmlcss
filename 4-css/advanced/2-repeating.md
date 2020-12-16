# Повторяющиеся свойства

- Свойства **не должны** повторяться в рамках одной декларации.
- Свойство **может** повторяться, если раньше описан сброс или общий случай.

### Правильно

```css
.block {
  margin: 0;
  margin-left: 20px;
  border: 10px solid #000000;
  border-bottom-color: #ff0000;
}
```

### Неправильно

```css
.block {
  margin-left: 10px;
  border-left: 10px solid #000000;
  margin-left: 20px;
  border-left: 10px solid #ff0000;
}
```
