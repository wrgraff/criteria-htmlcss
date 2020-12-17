# Неиспользуемый код

- В стилях **не должно** быть селекторов для элементов, которых нет в разметке ни одной из страниц.
- В стилях **могут** быть селекторы для тегов контентных блоков, которых пока нет в разметке.

## Правильно

```html
<div class="content">
  <h1>Привет, мир!</h1>
  <p>Волна когерентна.</p>
</div>
```

```css
.content h1 {
  font-size: 60px;
}

.content p {
  margin-bottom: 15px;
}

.content ul {
  padding-left: 50px;
  margin-left: 0;
}

.content table {
  width: 100%;
}
```

## Неправильно

```html
<div class="modal">
  <div class="modal__content"></div>
</div>
```

```css
.modal__overlay {
  position: absolute;
  background-color:rgba(0, 0, 0, 0.5);
}
```
