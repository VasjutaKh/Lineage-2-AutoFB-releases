# Шаблоны локаций телепорта (Community Board)

Поиск локаций: **panel.png** (вся сетка) → отдельная кнопка → OCR.

## Структура

```
templates/teleport/locations/
  aden/
    panel.png           ← вся колонка локаций (2×N кнопок)
    ivorytower.png      ← отдельная кнопка
    coliseum.png
    ...
  giran/
    panel.png
    ...
```

Имена файлов кнопок — без пробелов: `Ivory Tower` → `ivorytower.png`.

Порядок кнопок в сетке — в `vision/location_manifest.py`.

## Пересборка из скриншотов

```bash
uv run python scripts/build_location_templates.py
```

Скрипт читает исходные PNG из `assets/` (9 городов по порядку) и нарезает `panel.png` + кнопки.

## Как обновить один город

1. Положи новый скрин колонки локаций в `assets/`.
2. Обнови путь в `scripts/build_location_templates.py` или manifest.
3. Запусти скрипт пересборки.
