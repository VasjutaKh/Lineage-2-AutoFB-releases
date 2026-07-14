IbInputSimulator + Logitech G HUB + LGS
=========================================

Keyboard (F3 loot): Logitech G HUB (LogitechGHubNew)
Mouse clicks in L2: Logitech Gaming Software 9.02.65 (LGS)

WHY NOT MCII?
MCII kernel driver fails on Windows 11 24H2 (error 1450).
LGS uses Logitech virtual mouse driver — no kernel install.

SETUP
-----
1. Logitech G HUB — running as admin (keyboard)
2. IbInputSimulator.dll in vendor/IbInputSimulator/
3. LGS 9.02.65:
   launch\install_lgs.bat
   or vendor/IbInputSimulator/LGS_README.txt
4. Run game + bot as admin

TEST
----
  uv run python scripts/test_ib_input.py

Expected:
  1. G HUB ... OK
  2. Backend: LGS ... OK
