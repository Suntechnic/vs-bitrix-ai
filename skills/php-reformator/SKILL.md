---
name: php-reformator
description: "Reformat PHP code to match project conventions: rename variables with prefixes, fix braces, apply alternative syntax for HTML blocks, add strict_types. Use when refactoring or reformatting PHP files."
---

# PHP Reformator

## Procedure

Переформатируй текущий php файл в соответствии с соглашениями проекта:

1. Переименуй локально объявляемые и используемые переменные, согласно префиксам ($lst*, $dct*, $ref* и т.д.).
2. Перенеси открывающую фигурную скобку `{` блоков `if`, `foreach`, `while` и т.п. на ту же строку что и условие: `if ($Condition) {`
3. Оформи блоки if/foreach с HTML через альтернативный синтаксис (`:` / `end*`)
4. Однострочные guard-clause без фигурных скобок обязательны, если тело содержит только jump-оператор (`die`, `return`, `continue`, `break`, `include`).
5. Добавь в начало всех php файлов строгую типизацию `declare(strict_types=1);` и PHPDoc блок с входящими переменными, если его нет.

## Notes

После завершения всех изменений не предоставляй отчёт и не делай выводов. Сообщи только если возникли ошибки.
