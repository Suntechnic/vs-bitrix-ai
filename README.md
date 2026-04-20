# Bitrix AI

Agent-плагин для GitHub Copilot с соглашениями по PHP и Bitrix, скиллами для рефакторинга шаблонов и MCP-сервером Bitrix24.

## Требования

- VS Code с расширением GitHub Copilot
- Версия VS Code 1.100 или новее (поддержка agent plugins)

## Установка

1. Откройте Command Palette: `Ctrl+Shift+P`
2. Выполните команду: `Chat: Install Plugin From Source`
3. Введите URL репозитория:
   ```
   https://github.com/Suntechnic/vs-bitrix-ai.git
   ```
4. Дождитесь завершения установки.

После установки плагин активируется автоматически. Скиллы появятся в чате при вводе `/`.

## Обновление

1. Откройте Command Palette: `Ctrl+Shift+P`
2. Выполните команду: `Extensions: Check for Extension Updates`

Либо VS Code обновит плагин автоматически раз в 24 часа при включённой настройке `extensions.autoUpdate`.

## Удаление

1. Откройте панель Extensions: `Ctrl+Shift+X`
2. В поисковой строке введите `@agentPlugins`
3. Найдите **Bitrix AI** в списке установленных плагинов
4. Нажмите правой кнопкой → **Uninstall**

## Состав плагина

| Скилл | Команда | Описание |
|-------|---------|----------|
| `php` | авто | Соглашения по именованию переменных и стилю PHP-кода |
| `bitrix-php` | авто | Соглашения по PHP-тегам, Bitrix-сущностям и HTML-атрибутам |
| `php-reformator` | `/php-reformator` | Переформатирование PHP-файла под соглашения проекта |
| `bx-tint` | `/bx-tint` | Интеграция HTML-верстки в шаблон компонента Bitrix |
| `bx-trf` | `/bx-trf` | Переформатирование шаблона компонента Bitrix |

MCP-сервер Bitrix24 подключается автоматически при активации плагина.

