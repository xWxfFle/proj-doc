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
2. собирает MkDocs;
3. публикует сайт на GitHub Pages.

Включите Pages: **Settings → Pages → Source: GitHub Actions**.

## Участие

См. [CONTRIBUTING.md](CONTRIBUTING.md).
