# Неиспользуемый код

В скриптах не должно быть неиспользуемых переменных и функций.

## Правильно

```js
/* Modal */

const modalOverlay = document.querySelectorAll('.modal__overlay');

modalOverlay.addEventListener('click', event => {
  event.preventDefault();
})
```

## Неправильно

```js
/* Modal */

const modalOverlay = document.querySelectorAll('.modal__overlay');
const modalContent = document.querySelectorAll('.modal__content');

modalOverlay.addEventListener('click', event => {
  event.preventDefault();
})
```
