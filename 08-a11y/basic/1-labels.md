# Описание элементов

## Контентная графика

- Теги `<img>` **должны** иметь атрибут `alt` с описанием изображения.
- Контентная SVG-графика в разметке **должна** иметь `role="img"` и описание изображения в атрибуте `arial-label`.

### Правильно

```html
<img src="hammer.jpg" width="640" height="320" alt="Молоток.">

<img src="line.png" width="800" height="2" alt="">

<svg width="367" height="152" role="img" aria-label="Барбершоп «Бородинский»">
  <use xlink:href="logo.svg"></use>
</svg>
```


### Неправильно

```html
<img src="hammer.jpg" width="640" height="320">

<img src="line.png" width="800" height="2">

<svg width="367" height="152">
  <use xlink:href="logo.svg"></use>
</svg>
```

## Интерактивные элементы

- Интерактивные элементы **должны** быть подписаны.
- Подпись **должна** быть связана с элементом и отображаться в дереве доступности.

### Правильно

```html
<a href="/">
	<img src="logo.svg" width="64" height="32" alt="Барбершоп «Бородинский».">
</a>

<a href="https://twitter.com/yolo">
	<span class="visually-hidden">Читайте нас в Твиттере</span>
</a>

<button type="button" aria-label="Закрыть окно."></button>

<label for="login-name">Имя</label>
<input type="text" id="login-name">
```

### Неправильно

```html
<a href="/">
	<img src="logo.svg" width="64" height="32" alt="">
</a>

<a href="https://twitter.com/yolo"></a>

<button type="button"></button>

Имя
<input type="text">
```
