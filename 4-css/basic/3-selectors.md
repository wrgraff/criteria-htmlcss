# Классы в селекторах

## Классы

- Названия классов **должны** состоять из английских слов.
- Название может состоять из нескольких слов, в таком случае слова разделяются одним дефисом.

### Правильно

```css
.header {}
.header-logo {}
.footer {}
.footer-social {}
```

### Неправильно

```css
.header--logo {}
.header__logo {}
.headerLogo {}
```

## ID

- В селекторах **не должно** быть `#id`.

### Неправильно

```css
#header {
  background-color: #000000;
}
```

## Теги

- Нормализация тега `<img>` разрешена.
- Использвать глобальные теги запрещено, за исключением `img`, `video`.

### Правильно

```css
img {
  max-width: 100%;
}
```


### Неправильно

```css
img {
  max-width: 100%;
  object-fit: cover;
}
```


## Вложенность

- В cелекторах **не должно** быть вложенности больше 2.

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

### Неправильно

```css
.menu-item .menu-link {
  color: #ff0000;
}
```
