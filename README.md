# style-guide-project

Стайлгайд технической документации веб/SaaS-продукта. Документация ведётся по подходу **Docs as Code**: Markdown + MkDocs + линтинг + CI/CD.

## Быстрый старт

```bash
pip install -r requirements.txt
npm install
mkdocs serve
```

Откройте <http://127.0.0.1:8000>.

## Команды

| Команда | Назначение |
| --- | --- |
| `mkdocs serve` | Локальный предпросмотр |
| `mkdocs build --strict` | Сборка сайта |
| `npm run lint` | Проверка Markdown |

## CI/CD

При push в `main` GitHub Actions:

1. запускает markdownlint;
2. собирает MkDocs Material;
3. публикует сайт на GitHub Pages.

Важно: в настройках репозитория в разделе **Settings → Pages → Build and deployment** должно быть выбрано **Source: GitHub Actions**.

Если выбран Deploy from a branch / folder `docs`, GitHub публикует сырой Markdown через Jekyll — без бокового меню Material и иногда с «кракозябрами» в кэше. После переключения на Actions сделайте hard refresh (Ctrl+F5).

## Участие

См. [как предложить изменение в руководство](CONTRIBUTING.md).
