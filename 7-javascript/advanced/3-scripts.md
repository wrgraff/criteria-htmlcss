# Подключение скриптов

- Скрипты **должны** подключаться перед закрывающим тегом `</body>` или иметь атрибут `defer`.

## Правильно

```html
    <!-- Контент -->
    <script src="gallery.js"></script>
    <script src="script.js"></script>
  </body>
</html>
```

## Правильно

```html
    <script defer src="gallery.js"></script>
    <script defer src="script.js"></script>
    <!-- Контент -->
  </body>
</html>
```
