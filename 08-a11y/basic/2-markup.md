# Декоративная графика в разметке

- Декоративная графика в разметке **должна** иметь пустой `alt=""`.
- Инлайновые SVG-иконки **должны** иметь атрибут `aria-hidden="true"`.

## Правильно

```html
<svg width="16" height="16" aria-hidden="true">
  <use href="sprite.svg#icon"></use>
</svg>

<img width="16" height="16" src="icon.svg" alt="">
```
