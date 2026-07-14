Logitech Gaming Software (LGS) — клики мыши в L2
=================================================

MCII не работает на Windows 11 24H2 (ошибка 1450).
Вместо kernel-драйвера используй старый LGS с драйвером мыши Logitech.

1. Скачай LGS 9.02.65 (x64):
   https://github.com/Chaoses-Ib/IbLogiSoftExt/releases/download/v0.1/LGS.v9.02.65_x64.exe

2. Установи от администратора.
   Logitech-мышь НЕ нужна — драйвер виртуальный.

3. G HUB оставь запущенным (для клавиш F3).
   LGS нужен только для кликов мыши через IbInputSimulator.

4. Запусти клиент и игру от администратора.

5. Проверка:
   uv run python scripts/test_ib_input.py

   Должно быть:
   2. Mouse (LGS) ... OK

Если LGS FAIL — переустанови LGS, перезагрузи ПК.
