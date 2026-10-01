[BayLauncher](../README.md) > Installing

# Installing

1. Download `BayLauncher-Setup-<version>.exe` only from the link on bacustomproducts.com or the BayLauncher page on
   GitHub. The page lists the file's SHA-256 checksum, so anyone who wants to can check the file is the one BA Custom
   Products published.
2. Run it. The setup is not digitally signed yet, so Windows may say "Windows protected your PC". Choose
   **More info** > **Run anyway**, only for the file from the official link. On Windows 11 with Smart App Control
   turned on, Windows may block the setup completely: contact BA Custom Products through bacustomproducts.com and we
   will walk you through it.
3. Approve the Windows prompt. Installing needs an administrator account; day to day, nothing runs as administrator.
4. The setup explains what BayLauncher does, shows the ways back to the desktop, asks you to accept the license
   agreement, and asks where to install (keep the folder it suggests).
5. On the last page, tick "Open the 'Back to the desktop' sheet to print", print it, and keep it next to the bay PC.

## What installing changes
- The program goes in `C:\Program Files\BA Custom Products\BayLauncher`, with a Start menu folder named BayLauncher
  and an entry in Settings > Apps > Installed apps.
- Nothing starts by itself and no Windows account is changed. The cards only take over an account after you choose
  **Turn on BayLauncher for this account** (see [Turning BayLauncher on and off for an account](turn-on-and-off.md)).

## If the setup warns you
The setup checks the PC first. It stops on 32-bit Windows, and it warns (you can still choose to install) on an ARM
PC, Windows Server, Windows older than Windows 10 version 22H2, a main screen smaller than 1280 x 720, or an account
that already starts another kiosk or launcher program instead of the desktop.

---
BayLauncher owner guide, version 2026-10-01 (BayLauncher 1.0.0). © 2026 BA Custom Products LLC.
