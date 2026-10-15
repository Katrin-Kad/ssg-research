# Результаты эксперимента (MkDocs + Material + mike)

[![docs](https://github.com/Katrin-Kad/ssg-research/actions/workflows/docs.yml/badge.svg)](https://github.com/Katrin-Kad/ssg-research/actions/workflows/docs.yml)

Сайт: https://Katrin-Kad.github.io/ssg-research/

## Локальный запуск

```bash
python -m virtualenv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve                  # предпросмотр
mkdocs build --strict         # проверка, как в CI
```

## Публикация версий

```bash
git tag v1.0 && git push origin v1.0      # CI опубликует v1.0 и алиас latest
# ... изменить результаты ...
git tag v1.1 && git push origin v1.1      # CI опубликует v1.1, latest -> v1.1
```

Теги отправляйте по одному и дожидайтесь завершения workflow.

## Лицензии

Код — MIT (`LICENSE`), текст и результаты — CC BY 4.0 (`LICENSE-CONTENT.md`).
