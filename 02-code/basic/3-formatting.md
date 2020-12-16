# Форматирование кода

Код проекта **должен** соответствовать параметрам EditorConfig, описанным в файле `.editorconfig` проекта.

## EditorConfig

```
root = true

[*]
charset = utf-8
end_of_line = lf
indent_size = 2
indent_style = space
insert_final_newline = true
trim_trailing_whitespace = true
```

## Правильно

```html
<ul>
∙∙<li>Пункт</li>
∙∙<li>Пункт</li>
</ul>
```

## Неправильно

```html
<ul>
→ <li>Пункт</li>
∙∙∙∙<li>Пункт</li>∙∙∙∙∙∙∙
</ul>
```
