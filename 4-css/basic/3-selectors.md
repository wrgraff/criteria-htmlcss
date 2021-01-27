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
.menu-link {
  color: #ff0000;
}

.menu-item-active .menu-link {
  color: #0000dd;
}
```

### Неправильно

```css
.menu-item .menu-link {
  color: #ff0000;
}
```
