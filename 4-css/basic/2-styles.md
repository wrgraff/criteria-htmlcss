# Подключение стилей

- Стили должны быть подключены с помощью тега `<link rel="stylesheet">`.
- Стили проекта **должны** быть подключены одним файлом в `<head>`.
- Сторонние стили **должны** быть подключены в `<head>` отдельно.
- Сторонние стили **должны** быть подключены до стилей проекта.
- В разметке **не должно** быть инлайновых стилей в `style=""` или в `<style>`.

## Правильно

```html
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap">
<link rel="stylesheet" href="index.min.css">
```

## Неправильно

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap');
```

```html
<link rel="stylesheet" href="header.css">
<link rel="stylesheet" href="main.css">
<link rel="stylesheet" href="footer.css">
```
