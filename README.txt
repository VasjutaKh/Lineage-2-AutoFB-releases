L2 Bot — краткая инструкция
===========================

Запуск: L2Bot.exe (от имени администратора, если не работают горячие клавиши в игре)

Требования:
- Windows 10/11
- Tesseract OCR: https://github.com/UB-Mannheim/tesseract/wiki
- Игра Lineage 2, окно 1920x1080 (или auto_scale в пресете)
- Logitech G HUB  + Logitech Gaming Software

Первый запуск:
1. Открой config.yaml — укажи путь к tesseract.exe
2. Запусти L2Bot.exe
3. Войди: Login и Password на текущий день (кнопка «Вставить»)
4. Выбери клиент и пресет в GUI

Горячие клавиши (по умолчанию в пресете):
- UP (стрелка вверх) — старт/стоп бота
- F10 — пауза
- F12 — выход из сессии бота

Папки рядом с L2Bot.exe (не удалять):
- _internal/   — библиотеки PyInstaller
- config/      — daily_auth.enc, auth.yaml.example
- presets/     — пресеты фарма
- templates/   — шаблоны OCR (таргет, HP, мобы)
- vendor/      — IbInputSimulator (DLL ставится отдельно, см. vendor/IbInputSimulator/)
- logs/        — bot.log (создаётся при работе)

Lu4 / G HUB: для клавиш через Logitech нужен IbInputSimulator.dll в vendor/IbInputSimulator/
