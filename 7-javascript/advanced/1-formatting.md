# Форматирование

- Код, отвечающий за разные задачи, **должен** быть выделен в группу комментарием.
- Переменные **должны** объявляться в начале каждой группы.

## Правильно

```js
/* Modal */

const modal = document.querySelectorAll('.modal');
const modalOverlay = document.querySelectorAll('.modal-overlay');

const modalInit() => {
  //
}

/* Map */

const map = document.querySelectorAll('.map');
const modalContent = document.querySelectorAll('.map-content');

const mapInit() => {
  //
}
```

## Неправильно

```js
const modal = document.querySelectorAll('.modal');
const modalOverlay = document.querySelectorAll('.modal-overlay')
const map = document.querySelectorAll('.map');
const modalContent = document.querySelectorAll('.modal-content');

const mapInit() => {
  //
}

const modalInit() => {
  //
}
```
