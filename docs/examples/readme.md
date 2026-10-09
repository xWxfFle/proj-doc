# Пример: хороший README

## Меню разделов

### О стайлгайде

- [Назначение и область применения](../about/purpose.md)
- [Как пользоваться стайлгайдом](../about/how-to-use.md)
- [Как предложить изменение в руководство](../contributing.md)

### Правила

- [Язык и тон](../rules/language.md)
- [Структура документов](../rules/structure.md)
- [Форматирование](../rules/formatting.md)
- [Терминология](../rules/terminology.md)
- [Примеры кода](../rules/code-examples.md)
- [Заголовки и списки](../rules/headings.md)
- [Доступность текста](../rules/accessibility.md)

### Примеры

- [Хороший README](../examples/readme.md)
- [Фрагмент руководства пользователя](../examples/user-guide.md)

### Лабораторная

- [Ответы на вопросы](../lab/answers.md)
- [Тестирование стайлгайда](../lab/testing.md)

[← На главную](../index.md)

Ниже — фрагмент README, составленный по правилам этого стайлгайда.

---

## Фрагмент: Project API Client

Библиотека для работы с API продукта из Python. Подходит разработчикам интеграций.

## Требования

- Python 3.11+
- Действующий API-ключ организации

## Установка

```bash
pip install project-api-client
```

## Быстрый старт

1. Создайте API-ключ в разделе **Настройки → Разработчикам**.
2. Сохраните ключ в переменную окружения `PROJECT_API_KEY`.
3. Выполните запрос списка проектов:

```python
from project_api import Client

client = Client(api_key="YOUR_API_KEY")
projects = client.projects.list()
print(projects)
```

Ожидаемый результат: список объектов с полями `id` и `name`.

## Дальше

- [Аутентификация](../rules/terminology.md)
- [Примеры кода](../rules/code-examples.md)

---

**Почему это соответствует стайлгайду:** есть аудитория, предусловия, нумерованные шаги, плейсхолдер секрета, ожидаемый результат.
