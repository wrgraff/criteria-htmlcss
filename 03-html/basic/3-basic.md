# Базовые части разметки

На страницах **должны** быть базовые части разметки:

- Современный тип документа `<!DOCTYPE html>`
- Корневой элемент `<html>` с языком документа `lang`
- Метаинформация `<head>`
- Заголовок документа `<title>`
- Кодировка документа `<meta charset="utf-8">`
- Тело документа `<body>`

## Правильно

```html
<!DOCTYPE html>
<html lang="ru">
  <head>
    <meta charset="utf-8">
    <title>Заголовок</title>
  </head>
  <body>Страница</body>
</html>
```

## Неправильно

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
  <title>Заголовок</title>
  Страница
</html>
```
