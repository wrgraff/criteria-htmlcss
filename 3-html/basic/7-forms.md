# Рабочие формы

- Формы **должны** быть рабочими и отправлять введённые данные.
- Поля формы **должны** находится внутри тега `<form>`.
- У формы **должен** быть указан атрибут `action`.
- В атрибуте `method` **должен** быть указан тип отправки данных.
- У полей **должен** быть явно указан тип с помощью атрибута `type`.
- Тип поля **должен** соответствовать вводу, если это не противоречит дизайну.
- У полей **должен** быть заполненный атрибут `name`.
- У полей **может** быть заполненный атрибут `value`.

Для тестирования формы **можно** использовать адрес `https://echo.htmlacademy.ru/`.

### Правильно

```html
<form action="https://echo.htmlacademy.ru/" method="post">
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

<form action="https://echo.htmlacademy.ru/" method="post">
  <label>
    Поиск
    <input type="search" name="query">
  </label>
  <button type="submit">Найти</button>
</form>
```

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
