# tutor-homepage

Персональная страница репетитора английского языка — Иван Гаманович.

Статический сайт без сборки: чистый HTML + CSS.

## Структура

```
index.html                  главная страница
styles.css                  общие стили (светлая и тёмная тема)
materials/                  раздел «Материалы»
  index.html                список материалов
  grammar-tenses.html       времена английского глагола
  vocabulary-topics.html    тематические подборки лексики
  speaking-questions.html   вопросы для разговорной практики
  ielts-writing-checklist.html  чек-лист IELTS Writing Task 2
articles/                   раздел «Статьи»
  index.html                список статей
  how-to-learn-words.html   как запоминать слова
  ielts-preparation-plan.html  план подготовки к IELTS
  common-mistakes.html      10 типичных ошибок
```

## Локальный запуск

```bash
python3 -m http.server 8000
# http://localhost:8000
```

## Публикация

Сайт раздаётся GitHub Pages напрямую из ветки:
**Settings → Pages → Source: Deploy from a branch →
ветка `claude/tutor-page-gh-pages-8njef1`, папка `/ (root)`**.

Любой пуш в эту ветку автоматически обновляет сайт — сборка не нужна.
Файл `.nojekyll` отключает обработку Jekyll, чтобы страницы отдавались как есть.

Адрес сайта: https://igmiller777.github.io/tutor-homepage/

## Как добавить материал или статью

1. Скопируйте любой существующий файл в `materials/` или `articles/`.
2. Замените заголовок, `<meta name="description">` и содержимое внутри `<article class="prose">`.
3. Добавьте карточку со ссылкой в `index.html` соответствующего раздела.
