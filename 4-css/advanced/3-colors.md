# Формат цветов

- Цвета **должны** записываться строчными в 6-значном формате HEX.
- Цвета **могут** записываться функциями `rgba` или `hsla`, если нужна прозрачность.

## Правильно

```css
.block {
	background-color: #ff0000;
  border-left-color: #00ff00;
  color: rgba(0, 0, 0, 0.5);
}
```

## Неправильно

```css
.block {
  background-color: #F00;
  border-left-color: rgb(0, 255, 0);
  color: black;
}
```
