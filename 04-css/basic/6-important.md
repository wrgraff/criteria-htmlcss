# Использование `!important`

- Ключевое слово `!important` **не должно** использоваться для борьбы со специфичностью.
- Универсальные классы-хелперы **могут** использовать `!important`.

## Правильно

```css
.visually-hidden {
  position: absolute !important;
  width: 1px !important;
  height: 1px !important;
  margin: -1px !important;
  border: 0 !important;
  padding: 0 !important;
  clip: rect(0 0 0 0) !important;
  overflow: hidden !important;
}
```
