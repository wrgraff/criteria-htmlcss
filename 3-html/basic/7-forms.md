# Работоспособные формы

- Формы **должны** быть работоспособными и отправлять введённые данные.
- Поля формы **должны** находится внутри тега `<form>`.
- У формы **должен** быть указан атрибут `action`.
- У полей **должен** быть явно указан тип с помощью атрибута `type`.
- У полей **должны** быть атрибуты `name`.

Для тестирования формы **можно** использовать адрес `https://echo.htmlacademy.ru/`.

### Правильно

```html
<form action="https://echo.htmlacademy.ru/">
  <label>
    Логин
    <input type="text" name="user">
  </label>
  <label>
    Пароль
    <input type="password" name="password">
  </label>
  <button type="submit">Отправить</button>
</form>

<form action="https://echo.htmlacademy.ru/">
  <label>
    Поиск
    <input type="search" name="query">
  </label>
  <button type="submit">Найти</button>
</form>
```

### Неправильно

```html
<form>
  <label>
    Логин
    <input type="text">
  </label>
  <label>
    Пароль
    <input type="text">
  </label>
  <button type="button">Отправить</button>
</form>

<label>
  Поиск
  <input>
</label>
<button type="submit">Найти</button>
```
