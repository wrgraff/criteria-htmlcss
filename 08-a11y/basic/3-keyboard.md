# Доступность с клавиатуры

- Все интерактивные элементы **должны** быть доступны с клавиатуры.
- Порядок фокуса на интерактивных элементах **не должен** изменяться стилями.

### Правильно

```html
<button class="button">Закрыть</button>
```

### Неправильно

```html
<div class="button">Закрыть</div>
```

### Правильно

```html
<nav class="menu">
  <a class="menu__item menu__item--current" href>Кроет</li>
  <a class="menu__item" href>Буря</li>
  <a class="menu__item" href>Мглою</li>
  <a class="menu__item" href>Небо</li>
</nav>
```

```css
.menu {
  display: grid;
}
```

```
• Кроет
• Буря
• Мглою
• Небо
```

### Неправильно

```html
<nav class="menu">
  <a class="menu__item" href>Буря</li>
  <a class="menu__item" href>Мглою</li>
  <a class="menu__item" href>Небо</li>
  <a class="menu__item menu__item--current" href>Кроет</li>
</nav>
```

```css
.menu {
  display: grid;
}

.menu__item--current {
  order: -1;
}
```

```
• Кроет
• Буря
• Мглою
• Небо
```
