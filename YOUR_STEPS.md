# Что сделать тебе вручную

Ниже только шаги, которые требуют твоего аккаунта GitHub / партнёра / браузера. Всё остальное по лабораторной уже подготовлено в репозитории.

## 6. Репозиторий `style-guide-project` на GitHub

1. Открой <https://github.com/new>
2. Repository name: `style-guide-project`
3. Public → Create repository (**без** README / .gitignore — они уже есть локально)
4. В папке проекта выполни:

```powershell
git remote rename origin old-origin
git remote add origin https://github.com/xWxfFle/style-guide-project.git
git push -u origin main
```

(Если логин не `xWxfFle` — подставь свой.)

1. Settings → Pages → Source: **GitHub Actions**

## 11. Pull Request и обмен ревью

Код ветки `feat/accessibility` уже готовится локально. После push `main`:

```powershell
git push -u origin feat/accessibility
```

На GitHub: **Compare & pull request** → base `main` ← compare `feat/accessibility`.

### 11.6–11.7 Обмен с партнёром

1. Скинь партнёру ссылку на свой PR.
2. Получи ссылку на его PR.
3. Оставь **минимум 3 комментария** (пример формулировок):
   - «В разделе доступности стоит добавить пример плохого alt-текста.»
   - «Предлагаю в чек-лист добавить проверку языка страницы (`lang`).»
   - «Вопрос: распространяются ли правила alt на диаграммы Mermaid?»

### 11.8 Правки по замечаниям

Внеси правки в той же ветке → новый коммит → push. CI перезапустится сам.

### 11.9 Merge

После Approve нажми **Merge pull request** → Confirm.

### 11.10 Деплой

Actions → дождись зелёного workflow **CI**.  
Pages: `https://<логин>.github.io/style-guide-project/`  
(если в Settings указан project site).

## Опционально: установить GitHub CLI

Чтобы дальше создавать PR из терминала:

```powershell
winget install GitHub.cli
gh auth login
```
