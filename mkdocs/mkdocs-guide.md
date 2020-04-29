# Гайд по MkDocs

1. Поставить на комп Python если не стоит ещё.
2. Через его консоль поставить mkdocs.
   `pip install mkdocs`
3. Всё управление идёт через консоль.
   - Новый проект (проект создаётся там, где запущена консоль).
     `mkdocs new my-project
     cd my-project`
   - Запуск живого превью (будет доступно по адресу http://127.0.0.1:8000/)
     `mkdocs serve`
   - Билдинг проекта в статичный сайт:
     `mkdocs build`
4. Вся работа с текстом идёт в файлах .md. Синтаксис markdown.
5. В файле mkdocs.yml все настройки проекта и его структура.
6. Я изменил дефолтные настройки на свои чтобы сайт билдился в папку docs которая используется в github pages. А рабочие файлы лежат в папке mkdocs.
7. После того как я отдам репозиторий, работа по изменению доков будет выглядеть так:
   1. Правки вносятся в файлы в папке mkdocs.
   2. Картинки добавляются в папку mkdocs/img.
   3. Робот у себя запускает билд сайта (см. выше).
   4. Робот делает пуш в мастер гита.
   5. Какое-то время это могу делать я.

## Дока по MkDocs

https://www.mkdocs.org/user-guide/configuration/

## Дока по Маркдаун

https://wordpress.com/support/markdown-quick-reference/