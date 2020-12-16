# Классы в селекторах

## Классы

- В записи классов **должна** использоваться нотация БЭМ.
- Описание элементов и модификаторов блока **должны** находиться в том же файле.
- Элементы в стилях компонента **должны** описываться после блока.
- Модификаторы в стилях компонента **должны** описываться после основных стилей.

### Правильно

```css
.block {}
.block--modifier {}
.block__element {}
.block__element--modifier {}
```

### Неправильно

```css
.block {}
.block-modifier {}
.block-element {}
.block-element-modifier {}
```

### Правильно

```css
.block {}
.block--modifier {}
.block__element {}
```

### Неправильно

```css
.block__element {}
.block--modifier {}
.block {}
```

## ID и теги

- В селекторах **не должно** быть тегов и `#id`.
- В контентных областях **могут** использоваться селекторы по тегам.

### Правильно

```css
.page {
  font-family: "Roboto", sans-serif;
}

.header {
  background-color: #000000;
}

.content p {
	margin-bottom: 20px;
}
```

### Неправильно

```css
body {
	font-family: "Roboto", sans-serif;
}

#header {
  background-color: #000000;
}

p {
  margin-bottom: 20px;
}
```

## Вложенность

- В cелекторах **не должно** быть вложенности.
- В селекторах **может** быть вложенность для стилизации контентных тегов.
- В селекторах **может** быть вложенность для модификации от вложенности.

### Правильно

```css
.content ul li {
	content: "—";
}

.content ol li {
	content: counter;
}
```

### Неправильно

```css
.navigation li {
	list-style: none;
}

.navigation li a {
	text-decoration: none;
}
```

### Правильно

```css
.menu__item--current .menu__link {
	color: #ff0000;
}
```

### Неправильно

```css
.menu__item .menu__link {
	color: #ff0000;
}
```
