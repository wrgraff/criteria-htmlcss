# Подписи к блокам

Подписи к блокам **должны** быть связаны с блоками атрибутами или структурой тегов.

## Правильно

```html
<label>
	Имя
  <input type="text">
</label>

<label for="name">Имя</label>
<input type="text" id="name">
```

## Неправильно

```html
Имя
<input type="text" name="name">
```

## Правильно

```html
<fieldset>
  <legend>Адрес</legend>
  <input type="text" name="city">
  <input type="text" name="street">
</fieldset>
```

## Неправильно

```html
Адрес
<input type="text" name="city">
<input type="text" name="street">
```

## Правильно

```html
<table>
  <caption>Прайс-лист</caption>
	…
</table>
```

## Неправильно

```html
<table>
	…
</table>
Прайс-лист
```

## Правильно

```html
<figure>
  <img src="" alt="Отбойный молоток.">
  <figcaption>Фото Ирины Кравцовой.</figcaption>
</figure>
```

## Неправильно

```html
<img src="" alt="Отбойный молоток.">
<p>Фото Ирины Кравцовой.</p>
```
