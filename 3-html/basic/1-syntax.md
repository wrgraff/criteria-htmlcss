# Синтаксис

## Теги

- Имена тегов и атрибуты **должны** быть записаны строчными буквами.
- Двойные теги **должны** иметь открывающий и закрывающий теги.
- Одиночные теги **не должны** иметь закрывающий тег или слэш.

### Правильно

```html
<ul>
  <li>Первый</li>
  <li>Второй</li>
  <li>Третий</li>
</ul>

<img src="picture.png" alt="…">

<input type="text">
```

### Неправильно

```html
<UL>
  <LI>Первый
  <LI>Второй
  <LI>Третий
</UL>

<img src="picture.png" alt="…" />

<input type="text"></input>
```

## Атрибуты

- Имена атрибутов **должны** быть записаны строчными буквами.
- Атрибуты **должны** идти в одном порядке, чтобы упростить их чтение.
- Одиночные атрибуты **должны** быть записаны без значения.
- В записи атрибутов **не должно** быть пробелов вокруг знака «равно» `=`.
- Значения атрибутов **должны** быть в двойных кавычках.
- Вложенные кавычки в значениях **должны** быть одиночными.
- В атрибутах **не должно** быть единиц измерения.

### Правильно

```html
<form>
  <input type="text" required>
  <input type="email">
  <input type="tel" disabled>
</form>

<button class="button" type="button" onclick="show('menu')">
  Меню
</button>

<img src="picture.png" width="100" height="100" alt="">
```

### Неправильно

```html
<FORM>
  <input type="text" REQUIRED>
  <input type = "email">
  <input disabled="disabled" type="tel">
</FORM>

<button class=button type=button onclick='show("menu")'>
  Меню
</button>

<img src="picture.png" width="100%" height="100px" alt="">
```

## Классы

- Атрибут `class` **должен** идти сразу после имени тега.
- Значение класса **должно** быть записано строчными буквами.
- Разделителями в имени класса **должны** быть только дефисы `-` и подчёркивания `_`.

### Правильно

```html
<form class="form" method="post">
  <input class="form-input form-input-name" type="text">
  <input class="form-input form-input-password" type="password">
</form>
```

### Неправильно

```html
<form>
  <input type="text" class="FormInput FormInputName">
  <input type="password" class="FormInput FormInputPassword">
</form>
```
